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

## Class CxxPreprocessAndCompile {#class-cxxpreprocessandcompile .title title="Class CxxPreprocessAndCompile"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<com.facebook.buck.cxx.CxxPreprocessAndCompile.Impl\>

        -   -   com.facebook.buck.cxx.CxxPreprocessAndCompile

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `SupportsDependencyFileRuleKey`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`, `CxxIntermediateBuildProduct`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CxxPreprocessAndCompile
        extends ModernBuildRule<com.facebook.buck.cxx.CxxPreprocessAndCompile.Impl>
        implements SupportsDependencyFileRuleKey, CxxIntermediateBuildProduct

    ::: block
    A build rule which preprocesses and/or compiles a C/C++ source in a
    single step.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Cxx           | `compile​(             |                       |
        | PreprocessAndCompile` | BuildTarget buildTarg |                       |
        |                       | et,        ProjectFil |                       |
        |                       | esystem projectFilesy |                       |
        |                       | stem,        SourcePa |                       |
        |                       | thRuleFinder ruleFind |                       |
        |                       | er,        com.facebo |                       |
        |                       | ok.buck.cxx.CompilerD |                       |
        |                       | elegate compilerDeleg |                       |
        |                       | ate,        String ou |                       |
        |                       | tputName,        Sour |                       |
        |                       | cePath input,         |                       |
        |                       | CxxSource.Type inputT |                       |
        |                       | ype,        DebugPath |                       |
        |                       | Sanitizer sanitizer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCommand​(B         | ::: block             |
        | ogle.common.collect.I | uildContext context)` | Returns the           |
        | mmutableList<String>` |                       | compilation command   |
        |                       |                       | (used for compdb).    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getCov               | ::: block             |
        | redicate<SourcePath>` | eredByDepFilePredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | a given path is       |
        |                       |                       | covered by dep-file   |
        |                       |                       | or not.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getExiste            | ::: block             |
        | redicate<SourcePath>` | nceOfInterestPredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | the existence of a    |
        |                       |                       | given path may be of  |
        |                       |                       | interest to compiler. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getInput()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getInputsAf          | ::: block             |
        | .common.collect.Immut | terBuildingLocally​(Bu | Returns a list of     |
        | ableList<SourcePath>` | ildContext context,   | source paths that     |
        |                       |                       | were actually used    |
        |                       |        CellPathResolv | for the rule.         |
        |                       | er cellPathResolver)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSourceInpu        | ::: block             |
        |                       | tPath​(SourcePathResol | Returns the original  |
        |                       | verAdapter resolver)` | path of the source    |
        |                       |                       | file relative to its  |
        |                       |                       | own project root      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.face             | `make                 |                       |
        | book.buck.cxx.CxxPrep | MainStep​(BuildContext |                       |
        | rocessAndCompileStep` |  context,             |                       |
        |                       |  boolean useArgFile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Cxx           | `preprocessAndCompile |                       |
        | PreprocessAndCompile` | ​(BuildTarget buildTar |                       |
        |                       | get,                  |                       |
        |                       |     ProjectFilesystem |                       |
        |                       |  projectFilesystem,   |                       |
        |                       |                    So |                       |
        |                       | urcePathRuleFinder ru |                       |
        |                       | leFinder,             |                       |
        |                       |          com.facebook |                       |
        |                       | .buck.cxx.Preprocesso |                       |
        |                       | rDelegate preprocesso |                       |
        |                       | rDelegate,            |                       |
        |                       |           com.faceboo |                       |
        |                       | k.buck.cxx.CompilerDe |                       |
        |                       | legate compilerDelega |                       |
        |                       | te,                   |                       |
        |                       |    String outputName, |                       |
        |                       |                       |                       |
        |                       | SourcePath input,     |                       |
        |                       |                  CxxS |                       |
        |                       | ource.Type inputType, |                       |
        |                       |                       |                       |
        |                       | Optional<com.facebook |                       |
        |                       | .buck.cxx.CxxPrecompi |                       |
        |                       | ledHeader> precompile |                       |
        |                       | dHeaderRule,          |                       |
        |                       |             DebugPath |                       |
        |                       | Sanitizer sanitizer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `should               |                       |
        |                       | RespectInputSizeLimit |                       |
        |                       | ForRemoteExecution()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useDepe              |                       |
        |                       | ndencyFileRuleKeys()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, hasBuildSteps, hashCode, injectFields, isCacheable, toString`

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, toString, updateBuildRuleResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getType` in class `AbstractBuildRule`

        []{#compile(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.cxx.CompilerDelegate,java.lang.String,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.cxx.toolchain.DebugPathSanitizer)}

        -   #### compile

            ``` methodSignature
            public static CxxPreprocessAndCompile compile​(BuildTarget buildTarget,
                                                          ProjectFilesystem projectFilesystem,
                                                          SourcePathRuleFinder ruleFinder,
                                                          com.facebook.buck.cxx.CompilerDelegate compilerDelegate,
                                                          String outputName,
                                                          SourcePath input,
                                                          CxxSource.Type inputType,
                                                          DebugPathSanitizer sanitizer)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`CxxPreprocessAndCompile`](CxxPreprocessAndCompile.html "class in com.facebook.buck.cxx")
                step that compiles the given preprocessed source.

        []{#preprocessAndCompile(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.cxx.PreprocessorDelegate,com.facebook.buck.cxx.CompilerDelegate,java.lang.String,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.cxx.CxxSource.Type,java.util.Optional,com.facebook.buck.cxx.toolchain.DebugPathSanitizer)}

        -   #### preprocessAndCompile

            ``` methodSignature
            public static CxxPreprocessAndCompile preprocessAndCompile​(BuildTarget buildTarget,
                                                                       ProjectFilesystem projectFilesystem,
                                                                       SourcePathRuleFinder ruleFinder,
                                                                       com.facebook.buck.cxx.PreprocessorDelegate preprocessorDelegate,
                                                                       com.facebook.buck.cxx.CompilerDelegate compilerDelegate,
                                                                       String outputName,
                                                                       SourcePath input,
                                                                       CxxSource.Type inputType,
                                                                       Optional<com.facebook.buck.cxx.CxxPrecompiledHeader> precompiledHeaderRule,
                                                                       DebugPathSanitizer sanitizer)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`CxxPreprocessAndCompile`](CxxPreprocessAndCompile.html "class in com.facebook.buck.cxx")
                step that preprocesses and compiles the given source.

        []{#getSourceInputPath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getSourceInputPath

            ``` methodSignature
            public String getSourceInputPath​(SourcePathResolverAdapter resolver)
            ```

            ::: block
            Returns the original path of the source file relative to its
            own project root
            :::

        []{#getCommand(com.facebook.buck.core.build.context.BuildContext)}

        -   #### getCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommand​(BuildContext context)
            ```

            ::: block
            Returns the compilation command (used for compdb).
            :::

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<com.facebook.buck.cxx.CxxPreprocessAndCompile.Impl>`

        []{#getInput()}

        -   #### getInput

            ``` methodSignature
            public SourcePath getInput()
            ```

        []{#useDependencyFileRuleKeys()}

        -   #### useDependencyFileRuleKeys

            ``` methodSignature
            public boolean useDependencyFileRuleKeys()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `useDependencyFileRuleKeys` in
                interface `SupportsDependencyFileRuleKey`

        []{#getCoveredByDepFilePredicate(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCoveredByDepFilePredicate

            ``` methodSignature
            public java.util.function.Predicate<SourcePath> getCoveredByDepFilePredicate​(SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            [Description copied from
            interface: `SupportsDependencyFileRuleKey`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a predicate that can tell whether a given path is
            covered by dep-file or not. Note that being covered by
            dep-file doesn\'t necessarily mean being present in the
            dep-file. A covered path will only be present if actually
            used and that\'s the core idea of dep-file keys.
            I.e. this predicate should return true only for source paths
            that \*may\* be returned from
            [`SupportsDependencyFileRuleKey.getInputsAfterBuildingLocally(BuildContext, CellPathResolver)`](../core/rules/attr/SupportsDependencyFileRuleKey.html#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)).
            This information is used by the rule key builder to infer
            that inputs \*not\* in this list should be included
            unconditionally in the rule key. Inputs that \*are\* in this
            list should be included in the rule key if and only if they
            are actually being used for the rule. I.e. if they are
            present in the dep-file listed by
            [`SupportsDependencyFileRuleKey.getInputsAfterBuildingLocally(BuildContext, CellPathResolver)`](../core/rules/attr/SupportsDependencyFileRuleKey.html#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCoveredByDepFilePredicate` in
                interface `SupportsDependencyFileRuleKey`

        []{#getExistenceOfInterestPredicate(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getExistenceOfInterestPredicate

            ``` methodSignature
            public java.util.function.Predicate<SourcePath> getExistenceOfInterestPredicate​(SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            [Description copied from
            interface: `SupportsDependencyFileRuleKey`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a predicate that can tell whether the existence of a
            given path may be of interest to compiler. If this predicate
            returns true, the path should be included in the rule key.
            Note that we only care about the existence here. The actual
            content of the file is not relevant.
            The main purpose of this predicate is to support scenarios
            where compiler decides whether to use a file or not solely
            based on its path. Of course, if compiler decides to use the
            file, it should list it in the dep-file in which case both
            the path and the content will be included in the rule key.
            However, relying only on presence in the dep-file for such
            paths is not sufficient. The problem occurs when a new such
            file just gets added, in which case it won\'t be present in
            the dep-file produced in the previous build, and yet if we
            run a local build now the compiler may decide to use it. For
            that reason rule key needs to reflect existence of all such
            files and change when a such a file gets added or removed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExistenceOfInterestPredicate` in
                interface `SupportsDependencyFileRuleKey`

        []{#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### getInputsAfterBuildingLocally

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getInputsAfterBuildingLocally​(BuildContext context,
                                                                                                     CellPathResolver cellPathResolver)
                                                                                              throws IOException
            ```

            ::: block
            [Description copied from
            interface: `SupportsDependencyFileRuleKey`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a list of source paths that were actually used for
            the rule. This list comes from the dep-file produced by
            compiler.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputsAfterBuildingLocally` in
                interface `SupportsDependencyFileRuleKey`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#shouldRespectInputSizeLimitForRemoteExecution()}

        -   #### shouldRespectInputSizeLimitForRemoteExecution

            ``` methodSignature
            public final boolean shouldRespectInputSizeLimitForRemoteExecution()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldRespectInputSizeLimitForRemoteExecution` in
                interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldRespectInputSizeLimitForRemoteExecution` in
                interface `BuildRule`

            [Returns:]{.returnLabel}
            :   true if this rule should only be allowed to be executed
                via Remote Execution if it satisfies input size limits.

        []{#makeMainStep(com.facebook.buck.core.build.context.BuildContext,boolean)}

        -   #### makeMainStep

            ``` methodSignature
            public com.facebook.buck.cxx.CxxPreprocessAndCompileStep makeMainStep​(BuildContext context,
                                                                                  boolean useArgFile)
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
