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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Class JsFile\<T extends com.facebook.buck.features.js.JsFile.AbstractImpl\> {#class-jsfilet-extends-com.facebook.buck.features.js.jsfile.abstractimpl .title title="Class JsFile"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   com.facebook.buck.features.js.JsFile\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class JsFile<T extends com.facebook.buck.features.js.JsFile.AbstractImpl>
        extends ModernBuildRule<T>

    ::: block
    JS file rule converted to MBR
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `create​(BuildTarget   | ::: block             |
        | tic JsFile<com.facebo |  buildTarget,       P | Creates JS file       |
        | ok.buck.features.js.J | rojectFilesystem proj | release rule          |
        | sFile.JsFileRelease>` | ectFilesystem,        | implementation        |
        |                       | SourcePathRuleFinder  | :::                   |
        |                       | ruleFinder,       Opt |                       |
        |                       | ional<Arg> extraJson, |                       |
        |                       |        WorkerTool wor |                       |
        |                       | ker,       BuildTarge |                       |
        |                       | tSourcePath devFile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static JsFile<com.fa | `create               | ::: block             |
        | cebook.buck.features. | ​(BuildTarget buildTar | Creates JS file dev   |
        | js.JsFile.JsFileDev>` | get,       ProjectFil | rule implementation   |
        |                       | esystem projectFilesy | :::                   |
        |                       | stem,       SourcePat |                       |
        |                       | hRuleFinder ruleFinde |                       |
        |                       | r,       Optional<Arg |                       |
        |                       | > extraJson,       Wo |                       |
        |                       | rkerTool worker,      |                       |
        |                       |   SourcePath src,     |                       |
        |                       |    Optional<String> s |                       |
        |                       | ubPath,       Optiona |                       |
        |                       | l<Path> virtualPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `B                    | `get                  |                       |
        | uildTargetSourcePath` | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public BuildTargetSourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<T extends com.facebook.buck.features.js.JsFile.AbstractImpl>`

        []{#create(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional,com.facebook.buck.shell.WorkerTool,com.facebook.buck.core.sourcepath.SourcePath,java.util.Optional,java.util.Optional)}

        -   #### create

            ``` methodSignature
            public static JsFile<com.facebook.buck.features.js.JsFile.JsFileDev> create​(BuildTarget buildTarget,
                                                                                        ProjectFilesystem projectFilesystem,
                                                                                        SourcePathRuleFinder ruleFinder,
                                                                                        Optional<Arg> extraJson,
                                                                                        WorkerTool worker,
                                                                                        SourcePath src,
                                                                                        Optional<String> subPath,
                                                                                        Optional<Path> virtualPath)
            ```

            ::: block
            Creates JS file dev rule implementation
            :::

        []{#create(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional,com.facebook.buck.shell.WorkerTool,com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### create

            ``` methodSignature
            public static JsFile<com.facebook.buck.features.js.JsFile.JsFileRelease> create​(BuildTarget buildTarget,
                                                                                            ProjectFilesystem projectFilesystem,
                                                                                            SourcePathRuleFinder ruleFinder,
                                                                                            Optional<Arg> extraJson,
                                                                                            WorkerTool worker,
                                                                                            BuildTargetSourcePath devFile)
            ```

            ::: block
            Creates JS file release rule implementation
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
