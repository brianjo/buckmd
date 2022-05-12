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

## Class PreInclude {#class-preinclude .title title="Class PreInclude"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.cxx.PreInclude

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `CxxPreprocessorDep`, `NativeLinkableGroup`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CxxPrecompiledHeaderTemplate`, `CxxPrefixHeader`

    ------------------------------------------------------------------------

        public abstract class PreInclude
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements NativeLinkableGroup, CxxPreprocessorDep

    ::: block
    Represents a precompilable header file, along with dependencies.
    Rules which depend on this will inherit this rule\'s of
    dependencies. For example if a given rule R uses a precompiled
    header rule P, then all of P\'s `deps` will get merged into R\'s
    `deps` list.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected c          | `buildPrepr           |                       |
        | om.facebook.buck.cxx. | ocessorDelegate​(CxxPl |                       |
        | PreprocessorDelegate` | atform cxxPlatform,   |                       |
        |                       |                       |                       |
        |                       |    Preprocessor prepr |                       |
        |                       | ocessor,              |                       |
        |                       |              CxxToolF |                       |
        |                       | lags preprocessorFlag |                       |
        |                       | s,                    |                       |
        |                       |        ActionGraphBui |                       |
        |                       | lder graphBuilder,    |                       |
        |                       |                       |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get                  |                       |
        |                       | AbsoluteHeaderPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getCxxPreprocessor   |                       |
        | <CxxPreprocessorDep>` | Deps​(CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |           BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | CxxPreprocessorInput` | getCxxPreprocessorInp | Returns the           |
        |                       | ut​(CxxPlatform cxxPla | preprocessor input    |
        |                       | tform,                | that represents this  |
        |                       |          ActionGraphB | rule\'s public        |
        |                       | uilder graphBuilder)` | (exported)            |
        |                       |                       | declarations.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `g                    |                       |
        |                       | etHeaderSourcePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkable`      | `getNative            |                       |
        |                       | Linkable​(CxxPlatform  |                       |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract c           | `getPrecompiledHeader |                       |
        | om.facebook.buck.cxx. | ​(boolean canPrecompil |                       |
        | CxxPrecompiledHeader` | e,                    |                       |
        |                       |   com.facebook.buck.c |                       |
        |                       | xx.PreprocessorDelega |                       |
        |                       | te preprocessorDelega |                       |
        |                       | teForCxxRule,         |                       |
        |                       |              Dependen |                       |
        |                       | cyAggregation aggrega |                       |
        |                       | tedPreprocessDepsRule |                       |
        |                       | ,                     |                       |
        |                       |  CxxToolFlags compute |                       |
        |                       | dCompilerFlags,       |                       |
        |                       |                java.u |                       |
        |                       | til.function.Function |                       |
        |                       | <CxxToolFlags,​String> |                       |
        |                       |  getHash,             |                       |
        |                       |          java.util.fu |                       |
        |                       | nction.Function<CxxTo |                       |
        |                       | olFlags,​String> getBa |                       |
        |                       | seHash,               |                       |
        |                       |        CxxPlatform cx |                       |
        |                       | xPlatform,            |                       |
        |                       |           CxxSource.T |                       |
        |                       | ype sourceType,       |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList<String>  |                       |
        |                       | sourceFlags,          |                       |
        |                       |             ActionGra |                       |
        |                       | phBuilder graphBuilde |                       |
        |                       | r,                    |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRelativeHe        |                       |
        |                       | aderPath​(ProjectFiles |                       |
        |                       | ystem relativizedTo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTransitiveCxxPrep | ::: block             |
        | .common.collect.Immut | rocessorInput​(CxxPlat | Returns all           |
        | ableMap<BuildTarget,​C | form cxxPlatform,     | transitive            |
        | xxPreprocessorInput>` |                       | preprocessor inputs   |
        |                       |          ActionGraphB | for this library.     |
        |                       | uilder graphBuilder)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected D          | `requ                 | ::: block             |
        | ependencyAggregation` | ireAggregatedDepsRule | Find or create a      |
        |                       | ​(CxxPlatform cxxPlatf | [`Dependency          |
        |                       | orm,                  | Aggregation`](../core |
        |                       |          ActionGraphB | /rules/impl/Dependenc |
        |                       | uilder graphBuilder)` | yAggregation.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.rules.impl") |
        |                       |                       | rule, representing a  |
        |                       |                       | grouping of           |
        |                       |                       | dependencies:         |
        |                       |                       | generally, those deps |
        |                       |                       | from the current      |
        |                       |                       | [`CxxPl               |
        |                       |                       | atform`](toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected c          | `req                  | ::: block             |
        | om.facebook.buck.cxx. | uirePrecompiledHeader | Look up or build a    |
        | CxxPrecompiledHeader` | ​(boolean canPrecompil | precompiled header    |
        |                       | e,                    | build rule which this |
        |                       |       com.facebook.bu | build rule is         |
        |                       | ck.cxx.PreprocessorDe | requesting.           |
        |                       | legate preprocessorDe | :::                   |
        |                       | legate,               |                       |
        |                       |            CxxPlatfor |                       |
        |                       | m cxxPlatform,        |                       |
        |                       |                   Cxx |                       |
        |                       | Source.Type sourceTyp |                       |
        |                       | e,                    |                       |
        |                       |       CxxToolFlags co |                       |
        |                       | mpilerFlags,          |                       |
        |                       |                 DepsB |                       |
        |                       | uilder depsBuilder,   |                       |
        |                       |                       |                       |
        |                       |   BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hashCode, injectFields, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxPreprocessorDep}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxPreprocessorDep](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHeaderSourcePath()}

        -   #### getHeaderSourcePath

            ``` methodSignature
            public SourcePath getHeaderSourcePath()
            ```

            [Returns:]{.returnLabel}
            :   source path as specified in a
                `cxx_precompiled_header`\'s `src` attribute, or of a
                rule\'s `prefix_header`.

        []{#getAbsoluteHeaderPath()}

        -   #### getAbsoluteHeaderPath

            ``` methodSignature
            public Path getAbsoluteHeaderPath()
            ```

            [Returns:]{.returnLabel}
            :   path to the header file, guaranteed absolute

        []{#getRelativeHeaderPath(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getRelativeHeaderPath

            ``` methodSignature
            public Path getRelativeHeaderPath​(ProjectFilesystem relativizedTo)
            ```

            [Returns:]{.returnLabel}
            :   path to the header file, relativized against the given
                project filesystem (cell)

        []{#getNativeLinkable(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkable

            ``` methodSignature
            public NativeLinkable getNativeLinkable​(CxxPlatform cxxPlatform,
                                                    ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkable` in interface `NativeLinkableGroup`

        []{#getCxxPreprocessorDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getCxxPreprocessorDeps

            ``` methodSignature
            public Iterable<CxxPreprocessorDep> getCxxPreprocessorDeps​(CxxPlatform cxxPlatform,
                                                                       BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPreprocessorDeps` in
                interface `CxxPreprocessorDep`

        []{#getCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getCxxPreprocessorInput

            ``` methodSignature
            public CxxPreprocessorInput getCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `CxxPreprocessorDep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the preprocessor input that represents this rule\'s
            public (exported) declarations. This includes any exported
            preprocessor flags, headers, etc.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPreprocessorInput` in
                interface `CxxPreprocessorDep`

        []{#getTransitiveCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getTransitiveCxxPreprocessorInput

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​CxxPreprocessorInput> getTransitiveCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                                                                                    ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `CxxPreprocessorDep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns all transitive preprocessor inputs for this library.
            This includes public headers (and exported preprocessor
            flags) of all exported dependencies.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveCxxPreprocessorInput` in
                interface `CxxPreprocessorDep`

        []{#requireAggregatedDepsRule(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### requireAggregatedDepsRule

            ``` methodSignature
            protected DependencyAggregation requireAggregatedDepsRule​(CxxPlatform cxxPlatform,
                                                                      ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Find or create a
            [`DependencyAggregation`](../core/rules/impl/DependencyAggregation.html "class in com.facebook.buck.core.rules.impl")
            rule, representing a grouping of dependencies: generally,
            those deps from the current
            [`CxxPlatform`](toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
            :::

        []{#buildPreprocessorDelegate(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.Preprocessor,com.facebook.buck.cxx.CxxToolFlags,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### buildPreprocessorDelegate

            ``` methodSignature
            protected com.facebook.buck.cxx.PreprocessorDelegate buildPreprocessorDelegate​(CxxPlatform cxxPlatform,
                                                                                           Preprocessor preprocessor,
                                                                                           CxxToolFlags preprocessorFlags,
                                                                                           ActionGraphBuilder graphBuilder,
                                                                                           SourcePathResolverAdapter pathResolver)
            ```

            [Returns:]{.returnLabel}
            :   newly-built delegate for this PCH build (if precompiling
                enabled)

        []{#getPrecompiledHeader(boolean,com.facebook.buck.cxx.PreprocessorDelegate,com.facebook.buck.core.rules.impl.DependencyAggregation,com.facebook.buck.cxx.CxxToolFlags,java.util.function.Function,java.util.function.Function,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getPrecompiledHeader

            ``` methodSignature
            public abstract com.facebook.buck.cxx.CxxPrecompiledHeader getPrecompiledHeader​(boolean canPrecompile,
                                                                                            com.facebook.buck.cxx.PreprocessorDelegate preprocessorDelegateForCxxRule,
                                                                                            DependencyAggregation aggregatedPreprocessDepsRule,
                                                                                            CxxToolFlags computedCompilerFlags,
                                                                                            java.util.function.Function<CxxToolFlags,​String> getHash,
                                                                                            java.util.function.Function<CxxToolFlags,​String> getBaseHash,
                                                                                            CxxPlatform cxxPlatform,
                                                                                            CxxSource.Type sourceType,
                                                                                            com.google.common.collect.ImmutableList<String> sourceFlags,
                                                                                            ActionGraphBuilder graphBuilder,
                                                                                            SourcePathResolverAdapter pathResolver)
            ```

        []{#requirePrecompiledHeader(boolean,com.facebook.buck.cxx.PreprocessorDelegate,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.cxx.CxxToolFlags,com.facebook.buck.cxx.DepsBuilder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### requirePrecompiledHeader

            ``` methodSignature
            protected com.facebook.buck.cxx.CxxPrecompiledHeader requirePrecompiledHeader​(boolean canPrecompile,
                                                                                          com.facebook.buck.cxx.PreprocessorDelegate preprocessorDelegate,
                                                                                          CxxPlatform cxxPlatform,
                                                                                          CxxSource.Type sourceType,
                                                                                          CxxToolFlags compilerFlags,
                                                                                          DepsBuilder depsBuilder,
                                                                                          BuildTarget buildTarget,
                                                                                          ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Look up or build a precompiled header build rule which this
            build rule is requesting.
            This method will first try to determine whether a matching
            PCH was already created; if so, it will be reused. This is
            done by searching the cache in the
            [`ActionGraphBuilder`](../core/rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
            owned by this class. If this ends up building a new instance
            of `CxxPrecompiledHeader`, it will be added to the
            graphBuilder cache.
            :::
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
