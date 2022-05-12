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

## Class CxxThinLTOOpt {#class-cxxthinltoopt .title title="Class CxxThinLTOOpt"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[CxxThinLTOOpt.Impl](CxxThinLTOOpt.Impl.html "class in com.facebook.buck.cxx")\>

        -   -   com.facebook.buck.cxx.CxxThinLTOOpt

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `CxxIntermediateBuildProduct`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CxxThinLTOOpt
        extends ModernBuildRule<CxxThinLTOOpt.Impl>
        implements CxxIntermediateBuildProduct

    ::: block
    A build rule which runs the opt phase of an incremental ThinLTO
    build
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CxxThinLTOOpt.Impl`  | ::: block             |
        |                       |                       | Buildable             |
        |                       |                       | implementation for    |
        |                       |                       | CxxThinLTOOpt.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `getCommand​(B         | ::: block             |
        | ogle.common.collect.I | uildContext context)` | Returns the           |
        | mmutableList<String>` |                       | compilation command   |
        |                       |                       | (used for compdb).    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getInput()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `optimize​(B           |                       |
        | static CxxThinLTOOpt` | uildTarget buildTarge |                       |
        |                       | t,         ProjectFil |                       |
        |                       | esystem projectFilesy |                       |
        |                       | stem,         SourceP |                       |
        |                       | athRuleFinder ruleFin |                       |
        |                       | der,         com.face |                       |
        |                       | book.buck.cxx.Compile |                       |
        |                       | rDelegate compilerDel |                       |
        |                       | egate,         String |                       |
        |                       |  outputName,          |                       |
        |                       | SourcePath input,     |                       |
        |                       |      SourcePath thinI |                       |
        |                       | ndicesRoot,         C |                       |
        |                       | xxSource.Type inputTy |                       |
        |                       | pe,         DebugPath |                       |
        |                       | Sanitizer sanitizer)` |                       |
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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#optimize(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.cxx.CompilerDelegate,java.lang.String,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.cxx.CxxSource.Type,com.facebook.buck.cxx.toolchain.DebugPathSanitizer)}

        -   #### optimize

            ``` methodSignature
            public static CxxThinLTOOpt optimize​(BuildTarget buildTarget,
                                                 ProjectFilesystem projectFilesystem,
                                                 SourcePathRuleFinder ruleFinder,
                                                 com.facebook.buck.cxx.CompilerDelegate compilerDelegate,
                                                 String outputName,
                                                 SourcePath input,
                                                 SourcePath thinIndicesRoot,
                                                 CxxSource.Type inputType,
                                                 DebugPathSanitizer sanitizer)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`CxxThinLTOOpt`](CxxThinLTOOpt.html "class in com.facebook.buck.cxx")
                step that optimizes the given bitcode source.

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
                class `ModernBuildRule<CxxThinLTOOpt.Impl>`

        []{#getInput()}

        -   #### getInput

            ``` methodSignature
            public SourcePath getInput()
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
