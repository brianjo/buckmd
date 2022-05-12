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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class PreprocessorFlags {#class-preprocessorflags .title title="Class PreprocessorFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.PreprocessorFlags

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class PreprocessorFlags
        extends Object
        implements AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                         Description
          ------------------- ----------------------------- -------------
          `static class `     `PreprocessorFlags.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `PreprocessorFlags()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Prepr         | `builder()`           |                       |
        | ocessorFlags.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck    | `                     |                       |
        | .cxx.CxxIncludePaths` | getCxxIncludePaths()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `getDeps​(SourcePathRu |                       |
        |                       | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getFrameworkPaths()` | ::: block             |
        | bstract com.google.co |                       | Directories set via   |
        | mmon.collect.Immutabl |                       | `-F`.                 |
        | eList<FrameworkPath>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolFlags`        | `getIncludePa         |                       |
        |                       | thFlags​(SourcePathRes |                       |
        |                       | olverAdapter resolver |                       |
        |                       | ,                     |                       |
        |                       | PathShortener pathSho |                       |
        |                       | rtener,               |                       |
        |                       |       java.util.funct |                       |
        |                       | ion.Function<Framewor |                       |
        |                       | kPath,​Path> framework |                       |
        |                       | PathTransformer,      |                       |
        |                       |                Prepro |                       |
        |                       | cessor preprocessor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.google  | `getIncludes()`       | ::: block             |
        | .common.collect.Immut |                       | Directories set via   |
        | ableList<CxxHeaders>` |                       | `-I`.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolFlags`        | `getNonInclu          |                       |
        |                       | dePathFlags​(SourcePat |                       |
        |                       | hResolverAdapter reso |                       |
        |                       | lver,                 |                       |
        |                       |        Optional<Pair< |                       |
        |                       | com.facebook.buck.cxx |                       |
        |                       | .PrecompiledHeaderDat |                       |
        |                       | a,​PathShortener>> pch |                       |
        |                       | AndShortener,         |                       |
        |                       |                Prepro |                       |
        |                       | cessor preprocessor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolFlags`        | `getOtherFlags()`     | ::: block             |
        |                       |                       | Other flags included  |
        |                       |                       | as is.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getPrefixHeader()`   | ::: block             |
        | Optional<SourcePath>` |                       | File set via          |
        |                       |                       | `-include`.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolFlags`        | `g                    |                       |
        |                       | etSanitizedIncludePat |                       |
        |                       | hFlags​(DebugPathSanit |                       |
        |                       | izer sanitizer,       |                       |
        |                       |                       |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter resolver,      |                       |
        |                       |                       |                       |
        |                       |    PathShortener path |                       |
        |                       | Shortener,            |                       |
        |                       |                   jav |                       |
        |                       | a.util.function.Funct |                       |
        |                       | ion<FrameworkPath,​Pat |                       |
        |                       | h> frameworkPathTrans |                       |
        |                       | former,               |                       |
        |                       |                Prepro |                       |
        |                       | cessor preprocessor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of​(Optional<S        |                       |
        | ic PreprocessorFlags` | ourcePath> prefixHead |                       |
        |                       | er,   CxxToolFlags ot |                       |
        |                       | herFlags,   com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableList<CxxHeaders> |                       |
        |                       |  includes,   com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableList<FrameworkP |                       |
        |                       | ath> frameworkPaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxToolFlags`        | `t                    |                       |
        |                       | oToolFlags​(SourcePath |                       |
        |                       | ResolverAdapter resol |                       |
        |                       | ver,            PathS |                       |
        |                       | hortener pathShortene |                       |
        |                       | r,            java.ut |                       |
        |                       | il.function.Function< |                       |
        |                       | FrameworkPath,​Path> f |                       |
        |                       | rameworkPathTransform |                       |
        |                       | er,            Prepro |                       |
        |                       | cessor preprocessor,  |                       |
        |                       |            Optional<c |                       |
        |                       | om.facebook.buck.cxx. |                       |
        |                       | PrecompiledHeaderData |                       |
        |                       | > precompiledHeader)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PreprocessorFlags`   | `withFr               |                       |
        |                       | ameworkPaths​(com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableList<FrameworkP |                       |
        |                       | ath> frameworkPaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PreprocessorFlags`   | `withOtherFlags​(CxxT  |                       |
        |                       | oolFlags otherFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PreprocessorFlags`   | `withPrefix           |                       |
        |                       | Header​(Optional<Sourc |                       |
        |                       | ePath> prefixHeader)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PreprocessorFlags

                public PreprocessorFlags()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPrefixHeader()}

        -   #### getPrefixHeader

            ``` methodSignature
            public abstract Optional<SourcePath> getPrefixHeader()
            ```

            ::: block
            File set via `-include`. This might be a prefix header or a
            precompiled header.
            :::

        []{#getOtherFlags()}

        -   #### getOtherFlags

            ``` methodSignature
            @Default
            public CxxToolFlags getOtherFlags()
            ```

            ::: block
            Other flags included as is.
            :::

        []{#getIncludes()}

        -   #### getIncludes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<CxxHeaders> getIncludes()
            ```

            ::: block
            Directories set via `-I`.
            :::

        []{#getFrameworkPaths()}

        -   #### getFrameworkPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<FrameworkPath> getFrameworkPaths()
            ```

            ::: block
            Directories set via `-F`.
            :::

        []{#getCxxIncludePaths()}

        -   #### getCxxIncludePaths

            ``` methodSignature
            @Derived
            public com.facebook.buck.cxx.CxxIncludePaths getCxxIncludePaths()
            ```

        []{#getDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            public Iterable<BuildRule> getDeps​(SourcePathRuleFinder ruleFinder)
            ```

        []{#getIncludePathFlags(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.cxx.toolchain.PathShortener,java.util.function.Function,com.facebook.buck.cxx.toolchain.Preprocessor)}

        -   #### getIncludePathFlags

            ``` methodSignature
            public CxxToolFlags getIncludePathFlags​(SourcePathResolverAdapter resolver,
                                                    PathShortener pathShortener,
                                                    java.util.function.Function<FrameworkPath,​Path> frameworkPathTransformer,
                                                    Preprocessor preprocessor)
            ```

        []{#getSanitizedIncludePathFlags(com.facebook.buck.cxx.toolchain.DebugPathSanitizer,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.cxx.toolchain.PathShortener,java.util.function.Function,com.facebook.buck.cxx.toolchain.Preprocessor)}

        -   #### getSanitizedIncludePathFlags

            ``` methodSignature
            public CxxToolFlags getSanitizedIncludePathFlags​(DebugPathSanitizer sanitizer,
                                                             SourcePathResolverAdapter resolver,
                                                             PathShortener pathShortener,
                                                             java.util.function.Function<FrameworkPath,​Path> frameworkPathTransformer,
                                                             Preprocessor preprocessor)
            ```

        []{#getNonIncludePathFlags(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.util.Optional,com.facebook.buck.cxx.toolchain.Preprocessor)}

        -   #### getNonIncludePathFlags

            ``` methodSignature
            public CxxToolFlags getNonIncludePathFlags​(SourcePathResolverAdapter resolver,
                                                       Optional<Pair<com.facebook.buck.cxx.PrecompiledHeaderData,​PathShortener>> pchAndShortener,
                                                       Preprocessor preprocessor)
            ```

        []{#toToolFlags(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.cxx.toolchain.PathShortener,java.util.function.Function,com.facebook.buck.cxx.toolchain.Preprocessor,java.util.Optional)}

        -   #### toToolFlags

            ``` methodSignature
            public CxxToolFlags toToolFlags​(SourcePathResolverAdapter resolver,
                                            PathShortener pathShortener,
                                            java.util.function.Function<FrameworkPath,​Path> frameworkPathTransformer,
                                            Preprocessor preprocessor,
                                            Optional<com.facebook.buck.cxx.PrecompiledHeaderData> precompiledHeader)
            ```

        []{#of(java.util.Optional,com.facebook.buck.cxx.CxxToolFlags,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static PreprocessorFlags of​(Optional<SourcePath> prefixHeader,
                                               CxxToolFlags otherFlags,
                                               com.google.common.collect.ImmutableList<CxxHeaders> includes,
                                               com.google.common.collect.ImmutableList<FrameworkPath> frameworkPaths)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static PreprocessorFlags.Builder builder()
            ```

        []{#withFrameworkPaths(com.google.common.collect.ImmutableList)}

        -   #### withFrameworkPaths

            ``` methodSignature
            public PreprocessorFlags withFrameworkPaths​(com.google.common.collect.ImmutableList<FrameworkPath> frameworkPaths)
            ```

        []{#withOtherFlags(com.facebook.buck.cxx.CxxToolFlags)}

        -   #### withOtherFlags

            ``` methodSignature
            public PreprocessorFlags withOtherFlags​(CxxToolFlags otherFlags)
            ```

        []{#withPrefixHeader(java.util.Optional)}

        -   #### withPrefixHeader

            ``` methodSignature
            public PreprocessorFlags withPrefixHeader​(Optional<SourcePath> prefixHeader)
            ```
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
