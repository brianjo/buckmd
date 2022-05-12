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
[Package]{.packageLabelInType} [com.facebook.buck.features.halide](package-summary.html)
:::

## Class HalideLibrary {#class-halidelibrary .title title="Class HalideLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.features.halide.HalideLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `CxxPreprocessorDep`, `NativeLinkableGroup`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class HalideLibrary
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements CxxPreprocessorDep, NativeLinkableGroup
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                             Description
          -------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `HalideLibrary​(BuildTarget buildTarget,              ProjectFilesystem projectFilesystem,              BuildRuleParams params,              ActionGraphBuilder graphBuilder,              Optional<Pattern> supportedPlatformsRegex)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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
        | `NativeLinkableInfo`  | `getNative            |                       |
        |                       | Linkable​(CxxPlatform  |                       |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTransitiveCxxPrep | ::: block             |
        | .common.collect.Immut | rocessorInput​(CxxPlat | Returns all           |
        | ableMap<BuildTarget,​C | form cxxPlatform,     | transitive            |
        | xxPreprocessorInput>` |                       | preprocessor inputs   |
        |                       |          ActionGraphB | for this library.     |
        |                       | uilder graphBuilder)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxPreprocessorDep}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxPreprocessorDep](../../cxx/CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,java.util.Optional)}

        -   #### HalideLibrary

                protected HalideLibrary​(BuildTarget buildTarget,
                                        ProjectFilesystem projectFilesystem,
                                        BuildRuleParams params,
                                        ActionGraphBuilder graphBuilder,
                                        Optional<Pattern> supportedPlatformsRegex)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getNativeLinkable(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkable

            ``` methodSignature
            public NativeLinkableInfo getNativeLinkable​(CxxPlatform cxxPlatform,
                                                        ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkable` in interface `NativeLinkableGroup`
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
