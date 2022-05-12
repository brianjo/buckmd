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

## Class CxxPrecompiledHeaderTemplate {#class-cxxprecompiledheadertemplate .title title="Class CxxPrecompiledHeaderTemplate"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   [com.facebook.buck.cxx.PreInclude](PreInclude.html "class in com.facebook.buck.cxx")

                -   -   com.facebook.buck.cxx.CxxPrecompiledHeaderTemplate

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageable`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `BuildRule`, `HasNameAndType`, `CxxPreprocessorDep`,
        `NativeLinkableGroup`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CxxPrecompiledHeaderTemplate
        extends PreInclude
        implements AndroidPackageable

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
        | `void`                | `addToCollect         | ::: block             |
        |                       | or​(AndroidPackageable | Add concrete          |
        |                       | Collector collector)` | resources to the      |
        |                       |                       | given collector.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getPrecompiledHeader | ::: block             |
        | om.facebook.buck.cxx. | ​(boolean canPrecompil | Build a PCH rule,     |
        | CxxPrecompiledHeader` | e,                    | given a               |
        |                       |   com.facebook.buck.c | `cx                   |
        |                       | xx.PreprocessorDelega | x_precompiled_header` |
        |                       | te preprocessorDelega | rule.                 |
        |                       | teForCxxRule,         | :::                   |
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
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.PreInclude}

            ### Methods inherited from class com.facebook.buck.cxx.[PreInclude](PreInclude.html "class in com.facebook.buck.cxx")

            `buildPreprocessorDelegate, getAbsoluteHeaderPath, getCxxPreprocessorDeps, getCxxPreprocessorInput, getHeaderSourcePath, getNativeLinkable, getRelativeHeaderPath, getTransitiveCxxPreprocessorInput, requireAggregatedDepsRule, requirePrecompiledHeader`

        ```{=html}
        <!-- -->
        ```
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

        []{#getPrecompiledHeader(boolean,com.facebook.buck.cxx.PreprocessorDelegate,com.facebook.buck.core.rules.impl.DependencyAggregation,com.facebook.buck.cxx.CxxToolFlags,java.util.function.Function,java.util.function.Function,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxSource.Type,com.google.common.collect.ImmutableList,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getPrecompiledHeader

            ``` methodSignature
            public com.facebook.buck.cxx.CxxPrecompiledHeader getPrecompiledHeader​(boolean canPrecompile,
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

            ::: block
            Build a PCH rule, given a `cxx_precompiled_header` rule.
            We\'ll \"instantiate\" this PCH from this template, using
            the parameters (src, dependencies) from the template itself,
            plus the build flags that are used in the current build rule
            (so that this instantiated version uses compatible build
            flags and thus the PCH is guaranteed usable with this rule).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrecompiledHeader` in class `PreInclude`

        []{#getRequiredPackageables(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRequiredPackageables

            ``` methodSignature
            public Iterable<AndroidPackageable> getRequiredPackageables​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the set of packagables that need to be included in any
            package that includes this object.
            For example, an android_library will need all of its Java
            deps (except provided_deps), its resource deps, and its
            native library deps (even though it doesn\'t need the native
            library as a build-time dependency). An android_resource
            might need an android_library that declares a custom view
            that it references, as well as other android_resource rules
            that it references directly.

            TODO(natthu): Once build rules and buildables are merged,
            replace this method with another interface that lets an
            [`AndroidPackageable`](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredPackageables` in
                interface `AndroidPackageable`

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
                that must be included along with this one.

        []{#addToCollector(com.facebook.buck.android.packageable.AndroidPackageableCollector)}

        -   #### addToCollector

            ``` methodSignature
            public void addToCollector​(AndroidPackageableCollector collector)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Add concrete resources to the given collector.
            Implementations should call methods on the collector specify
            what concrete content must be included in an Android package
            that includes this object. For example, an android_library
            will add Java classes, an ndk_library will add native
            libraries, and android_resource will add resource
            directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToCollector` in interface `AndroidPackageable`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](../android/packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.
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
