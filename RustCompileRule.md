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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class RustCompileRule {#class-rustcompilerule .title title="Class RustCompileRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<com.facebook.buck.features.rust.RustCompileRule.Impl\>

        -   -   com.facebook.buck.features.rust.RustCompileRule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class RustCompileRule
        extends ModernBuildRule<com.facebook.buck.features.rust.RustCompileRule.Impl>

    ::: block
    Generate a rustc command line with all appropriate dependencies in
    place.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier              | Constructor           | Description           |
        +=======================+=======================+=======================+
        | `protected `          | `Ru                   | ::: block             |
        |                       | stCompileRule​(BuildTa | Work out how to       |
        |                       | rget buildTarget,     | invoke the Rust       |
        |                       |             ProjectFi | compiler, rustc.      |
        |                       | lesystem projectFiles | :::                   |
        |                       | ystem,                |                       |
        |                       |  SourcePathRuleFinder |                       |
        |                       |  ruleFinder,          |                       |
        |                       |        String filenam |                       |
        |                       | e,                Too |                       |
        |                       | l compiler,           |                       |
        |                       |       Linker linker,  |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList<Arg> arg |                       |
        |                       | s,                com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Arg>  |                       |
        |                       | depArgs,              |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | <Arg> linkerArgs,     |                       |
        |                       |             com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableSortedMap<String |                       |
        |                       | ,​Arg> environment,    |                       |
        |                       |              com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSortedMap<Sourc |                       |
        |                       | ePath,​Optional<String |                       |
        |                       | >> mappedSources,     |                       |
        |                       |             String ro |                       |
        |                       | otModule,             |                       |
        |                       |     com.facebook.buck |                       |
        |                       | .features.rust.RustBu |                       |
        |                       | ckConfig.RemapSrcPath |                       |
        |                       | s remapSrcPaths,      |                       |
        |                       |            Optional<S |                       |
        |                       | tring> xcrunSdkPath)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          -------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static RustCompileRule`   `from​(SourcePathRuleFinder ruleFinder,     BuildTarget buildTarget,     ProjectFilesystem projectFilesystem,     String filename,     Tool compiler,     Linker linker,     com.google.common.collect.ImmutableList<Arg> args,     com.google.common.collect.ImmutableList<Arg> depArgs,     com.google.common.collect.ImmutableList<Arg> linkerArgs,     com.google.common.collect.ImmutableSortedMap<String,​Arg> environment,     com.google.common.collect.ImmutableSortedMap<SourcePath,​Optional<String>> mappedSources,     String rootModule,     com.facebook.buck.features.rust.RustBuckConfig.RemapSrcPaths remapSrcPaths,     Optional<String> xcrunSdkPath)`    
          `protected static Path`    `getOutputDir​(BuildTarget target,             ProjectFilesystem filesystem)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               
          `SourcePath`               `getSourcePathToOutput()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.lang.String,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.cxx.toolchain.linker.Linker,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableSortedMap,java.lang.String,com.facebook.buck.features.rust.RustBuckConfig.RemapSrcPaths,java.util.Optional)}

        -   #### RustCompileRule

                protected RustCompileRule​(BuildTarget buildTarget,
                                          ProjectFilesystem projectFilesystem,
                                          SourcePathRuleFinder ruleFinder,
                                          String filename,
                                          Tool compiler,
                                          Linker linker,
                                          com.google.common.collect.ImmutableList<Arg> args,
                                          com.google.common.collect.ImmutableList<Arg> depArgs,
                                          com.google.common.collect.ImmutableList<Arg> linkerArgs,
                                          com.google.common.collect.ImmutableSortedMap<String,​Arg> environment,
                                          com.google.common.collect.ImmutableSortedMap<SourcePath,​Optional<String>> mappedSources,
                                          String rootModule,
                                          com.facebook.buck.features.rust.RustBuckConfig.RemapSrcPaths remapSrcPaths,
                                          Optional<String> xcrunSdkPath)

            ::: block
            Work out how to invoke the Rust compiler, rustc.
            In Rust, a crate is the equivalent of a package in other
            languages. It\'s also the basic unit of compilation.

            A crate can either be a \"binary crate\" - which generates
            an executable - or a \"library crate\", which makes an .rlib
            file. .rlib files contain both interface details (function
            signatures, inline functions, macros, etc) and compiled
            object code, and so are equivalent to both header files and
            library archives. There are also dynamic crates which
            compile to .so files.

            All crates are compiled from at least one source file, which
            is its main (or top, or root) module. It may have references
            to other modules, which may be in other source files. Rustc
            only needs the main module filename and will find the rest
            of the source files from there (akin to #include in C/C++).
            If the crate also has dependencies on other crates, then
            those .rlib files must also be passed to rustc for the
            interface details, and to be linked if its a binary crate.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.cxx.toolchain.linker.Linker,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableSortedMap,java.lang.String,com.facebook.buck.features.rust.RustBuckConfig.RemapSrcPaths,java.util.Optional)}

        -   #### from

            ``` methodSignature
            public static RustCompileRule from​(SourcePathRuleFinder ruleFinder,
                                               BuildTarget buildTarget,
                                               ProjectFilesystem projectFilesystem,
                                               String filename,
                                               Tool compiler,
                                               Linker linker,
                                               com.google.common.collect.ImmutableList<Arg> args,
                                               com.google.common.collect.ImmutableList<Arg> depArgs,
                                               com.google.common.collect.ImmutableList<Arg> linkerArgs,
                                               com.google.common.collect.ImmutableSortedMap<String,​Arg> environment,
                                               com.google.common.collect.ImmutableSortedMap<SourcePath,​Optional<String>> mappedSources,
                                               String rootModule,
                                               com.facebook.buck.features.rust.RustBuckConfig.RemapSrcPaths remapSrcPaths,
                                               Optional<String> xcrunSdkPath)
            ```

        []{#getOutputDir(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getOutputDir

            ``` methodSignature
            protected static Path getOutputDir​(BuildTarget target,
                                               ProjectFilesystem filesystem)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<com.facebook.buck.features.rust.RustCompileRule.Impl>`
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
