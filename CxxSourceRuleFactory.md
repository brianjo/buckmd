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

## Class CxxSourceRuleFactory {#class-cxxsourcerulefactory .title title="Class CxxSourceRuleFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxSourceRuleFactory

::: description
-   

    ------------------------------------------------------------------------

        @NotThreadSafe
        public abstract class CxxSourceRuleFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `CxxSourceRuleFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `checkPrefixAndPre    |                       |
        |                       | compiledHeaderArgs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `createCompileBuil    |                       |
        |                       | dTarget​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `c                    |                       |
        |                       | reateInferCaptureBuil |                       |
        |                       | dTarget​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `createOptimizeBuil   |                       |
        |                       | dTarget​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstrac    | `get                  |                       |
        | t ActionGraphBuilder` | ActionGraphBuilder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `                     |                       |
        | abstract BuildTarget` | getBaseBuildTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstract c | `getCompilerFlags()`  |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableMultimap |                       |                       |
        | <CxxSource.Type,​Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected ab         | `getCxxBuckConfig()`  |                       |
        | stract CxxBuckConfig` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getCxxPlatform()`    |                       |
        | abstract CxxPlatform` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstract   | `getCx                |                       |
        |  com.google.common.co | xPreprocessorInput()` |                       |
        | llect.ImmutableList<C |                       |                       |
        | xxPreprocessorInput>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `getFrameworks()`     |                       |
        | rotected com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.google | `getIncludes()`       |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<CxxHeaders>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `getPathResolver()`   |                       |
        | tected abstract Sourc |                       |                       |
        | ePathResolverAdapter` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getPicType()`        |                       |
        | ted abstract PicType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstract   | `ge                   | ::: block             |
        | Optional<SourcePath>` | tPrecompiledHeader()` | NOTE:                 |
        |                       |                       | `precompiled_header`  |
        |                       |                       | is incompatible with  |
        |                       |                       | `prefix_header`.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstract   | `getPrefixHeader()`   | ::: block             |
        | Optional<SourcePath>` |                       | NOTE: `prefix_header` |
        |                       |                       | is incompatible with  |
        |                       |                       | `precompiled_header`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getPreInclude()`     | ::: block             |
        | Optional<PreInclude>` |                       | Get (possibly         |
        |                       |                       | creating) the         |
        |                       |                       | [                     |
        |                       |                       | `PreInclude`](PreIncl |
        |                       |                       | ude.html "class in co |
        |                       |                       | m.facebook.buck.cxx") |
        |                       |                       | instance              |
        |                       |                       | corresponding to this |
        |                       |                       | rule\'s               |
        |                       |                       | `  prefix_header` or  |
        |                       |                       | `precompiled_header`, |
        |                       |                       | whichever is          |
        |                       |                       | applicable, or empty  |
        |                       |                       | if neither is used.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstra     | `ge                   |                       |
        | ct ProjectFilesystem` | tProjectFilesystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected j          | `g                    |                       |
        | ava.util.function.Fun | etSanitizeFunction()` |                       |
        | ction<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(ProjectFiles      |                       |
        | CxxSourceRuleFactory` | ystem projectFilesyst |                       |
        |                       | em,   BuildTarget bas |                       |
        |                       | eBuildTarget,   Actio |                       |
        |                       | nGraphBuilder actionG |                       |
        |                       | raphBuilder,   Source |                       |
        |                       | PathResolverAdapter p |                       |
        |                       | athResolver,   CxxBuc |                       |
        |                       | kConfig cxxBuckConfig |                       |
        |                       | ,   CxxPlatform cxxPl |                       |
        |                       | atform,   com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleList<CxxPreprocess |                       |
        |                       | orInput> cxxPreproces |                       |
        |                       | sorInput,   com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMultimap<CxxSour |                       |
        |                       | ce.Type,​Arg> compiler |                       |
        |                       | Flags,   Optional<Sou |                       |
        |                       | rcePath> prefixHeader |                       |
        |                       | ,   Optional<SourcePa |                       |
        |                       | th> precompiledHeader |                       |
        |                       | ,   PicType picType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cxx                  | `requireCompileB      |                       |
        | PreprocessAndCompile` | uildRule​(String name, |                       |
        |                       |                       |                       |
        |                       |    CxxSource source)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `require              |                       |
        | on.collect.ImmutableS | InferCaptureBuildRule |                       |
        | et<com.facebook.buck. | s​(com.google.common.c |                       |
        | cxx.CxxInferCapture>` | ollect.ImmutableMap<S |                       |
        |                       | tring,​CxxSource> sour |                       |
        |                       | ces,                  |                       |
        |                       |              InferBuc |                       |
        |                       | kConfig inferConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cxx                  | `requirePreprocessAnd |                       |
        | PreprocessAndCompile` | CompileBuildRule​(Stri |                       |
        |                       | ng name,              |                       |
        |                       |                       |                       |
        |                       |    CxxSource source)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `requirePreproce      |                       |
        | ommon.collect.Immutab | ssAndCompileRules​(com |                       |
        | leMap<CxxPreprocessAn | .google.common.collec |                       |
        | dCompile,​SourcePath>` | t.ImmutableMap<String |                       |
        |                       | ,​CxxSource> sources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `require              |                       |
        | m.google.common.colle | ThinOptRules​(com.goog |                       |
        | ct.ImmutableMap<CxxTh | le.common.collect.Imm |                       |
        | inLTOOpt,​SourcePath>` | utableMap<String,​CxxS |                       |
        |                       | ource> sources,       |                       |
        |                       |               SourceP |                       |
        |                       | ath thinIndicesRoot)` |                       |
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

        -   #### CxxSourceRuleFactory

                public CxxSourceRuleFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            protected abstract ProjectFilesystem getProjectFilesystem()
            ```

        []{#getBaseBuildTarget()}

        -   #### getBaseBuildTarget

            ``` methodSignature
            protected abstract BuildTarget getBaseBuildTarget()
            ```

        []{#getActionGraphBuilder()}

        -   #### getActionGraphBuilder

            ``` methodSignature
            protected abstract ActionGraphBuilder getActionGraphBuilder()
            ```

        []{#getPathResolver()}

        -   #### getPathResolver

            ``` methodSignature
            protected abstract SourcePathResolverAdapter getPathResolver()
            ```

        []{#getCxxBuckConfig()}

        -   #### getCxxBuckConfig

            ``` methodSignature
            protected abstract CxxBuckConfig getCxxBuckConfig()
            ```

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            protected abstract CxxPlatform getCxxPlatform()
            ```

        []{#getCxxPreprocessorInput()}

        -   #### getCxxPreprocessorInput

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableList<CxxPreprocessorInput> getCxxPreprocessorInput()
            ```

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableMultimap<CxxSource.Type,​Arg> getCompilerFlags()
            ```

        []{#getPrefixHeader()}

        -   #### getPrefixHeader

            ``` methodSignature
            protected abstract Optional<SourcePath> getPrefixHeader()
            ```

            ::: block
            NOTE: `prefix_header` is incompatible with
            `precompiled_header`.
            :::

        []{#getPrecompiledHeader()}

        -   #### getPrecompiledHeader

            ``` methodSignature
            protected abstract Optional<SourcePath> getPrecompiledHeader()
            ```

            ::: block
            NOTE: `precompiled_header` is incompatible with
            `prefix_header`.
            :::

        []{#getPicType()}

        -   #### getPicType

            ``` methodSignature
            protected abstract PicType getPicType()
            ```

        []{#checkPrefixAndPrecompiledHeaderArgs()}

        -   #### checkPrefixAndPrecompiledHeaderArgs

            ``` methodSignature
            @Check
            protected void checkPrefixAndPrecompiledHeaderArgs()
            ```

        []{#getPreInclude()}

        -   #### getPreInclude

            ``` methodSignature
            @Lazy
            protected Optional<PreInclude> getPreInclude()
            ```

            ::: block
            Get (possibly creating) the
            [`PreInclude`](PreInclude.html "class in com.facebook.buck.cxx")
            instance corresponding to this rule\'s `  prefix_header` or
            `precompiled_header`, whichever is applicable, or empty if
            neither is used.
            :::

            [See Also:]{.seeLabel}
            :   `PreIncludeFactory`

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            @Lazy
            protected com.google.common.collect.ImmutableSet<FrameworkPath> getFrameworks()
            ```

        []{#getIncludes()}

        -   #### getIncludes

            ``` methodSignature
            @Lazy
            protected com.google.common.collect.ImmutableList<CxxHeaders> getIncludes()
            ```

        []{#createOptimizeBuildTarget(java.lang.String)}

        -   #### createOptimizeBuildTarget

            ``` methodSignature
            public BuildTarget createOptimizeBuildTarget​(String name)
            ```

            [Returns:]{.returnLabel}
            :   a build target for a
                [`CxxThinLTOOpt`](CxxThinLTOOpt.html "class in com.facebook.buck.cxx")
                rule for the source with the given name.

        []{#createCompileBuildTarget(java.lang.String)}

        -   #### createCompileBuildTarget

            ``` methodSignature
            public BuildTarget createCompileBuildTarget​(String name)
            ```

            [Returns:]{.returnLabel}
            :   a build target for a
                [`CxxPreprocessAndCompile`](CxxPreprocessAndCompile.html "class in com.facebook.buck.cxx")
                rule for the source with the given name.

        []{#createInferCaptureBuildTarget(java.lang.String)}

        -   #### createInferCaptureBuildTarget

            ``` methodSignature
            public BuildTarget createInferCaptureBuildTarget​(String name)
            ```

        []{#getSanitizeFunction()}

        -   #### getSanitizeFunction

            ``` methodSignature
            @Lazy
            protected java.util.function.Function<String,​String> getSanitizeFunction()
            ```

        []{#requireCompileBuildRule(java.lang.String,com.facebook.buck.cxx.CxxSource)}

        -   #### requireCompileBuildRule

            ``` methodSignature
            public CxxPreprocessAndCompile requireCompileBuildRule​(String name,
                                                                   CxxSource source)
            ```

        []{#requireThinOptRules(com.google.common.collect.ImmutableMap,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### requireThinOptRules

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxThinLTOOpt,​SourcePath> requireThinOptRules​(com.google.common.collect.ImmutableMap<String,​CxxSource> sources,
                                                                                                              SourcePath thinIndicesRoot)
            ```

        []{#requirePreprocessAndCompileBuildRule(java.lang.String,com.facebook.buck.cxx.CxxSource)}

        -   #### requirePreprocessAndCompileBuildRule

            ``` methodSignature
            public CxxPreprocessAndCompile requirePreprocessAndCompileBuildRule​(String name,
                                                                                CxxSource source)
            ```

        []{#requireInferCaptureBuildRules(com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.InferBuckConfig)}

        -   #### requireInferCaptureBuildRules

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<com.facebook.buck.cxx.CxxInferCapture> requireInferCaptureBuildRules​(com.google.common.collect.ImmutableMap<String,​CxxSource> sources,
                                                                                                                               InferBuckConfig inferConfig)
            ```

        []{#requirePreprocessAndCompileRules(com.google.common.collect.ImmutableMap)}

        -   #### requirePreprocessAndCompileRules

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxPreprocessAndCompile,​SourcePath> requirePreprocessAndCompileRules​(com.google.common.collect.ImmutableMap<String,​CxxSource> sources)
            ```

        []{#of(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMultimap,java.util.Optional,java.util.Optional,com.facebook.buck.cxx.toolchain.PicType)}

        -   #### of

            ``` methodSignature
            public static CxxSourceRuleFactory of​(ProjectFilesystem projectFilesystem,
                                                  BuildTarget baseBuildTarget,
                                                  ActionGraphBuilder actionGraphBuilder,
                                                  SourcePathResolverAdapter pathResolver,
                                                  CxxBuckConfig cxxBuckConfig,
                                                  CxxPlatform cxxPlatform,
                                                  com.google.common.collect.ImmutableList<CxxPreprocessorInput> cxxPreprocessorInput,
                                                  com.google.common.collect.ImmutableMultimap<CxxSource.Type,​Arg> compilerFlags,
                                                  Optional<SourcePath> prefixHeader,
                                                  Optional<SourcePath> precompiledHeader,
                                                  PicType picType)
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
-   Nested \| 
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
