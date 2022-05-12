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

## Class CxxLink {#class-cxxlink .title title="Class CxxLink"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[CxxLink.Impl](CxxLink.Impl.html "class in com.facebook.buck.cxx")\>

        -   -   com.facebook.buck.cxx.CxxLink

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasSupplementaryOutputs`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`, `OverrideScheduleRule`,
        `HasAppleDebugSymbolDeps`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CxxLink
        extends ModernBuildRule<CxxLink.Impl>
        implements HasAppleDebugSymbolDeps, OverrideScheduleRule, HasSupplementaryOutputs

    ::: block
    A BuildRule for linking c++ objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CxxLink.Impl`        | ::: block             |
        |                       |                       | Buildable             |
        |                       |                       | implementation of     |
        |                       |                       | CxxLink.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CxxLink​(BuildTarget buildTarget,        ProjectFilesystem projectFilesystem,        SourcePathRuleFinder ruleFinder,        CellPathResolver cellResolver,        Linker linker,        Path output,        com.google.common.collect.ImmutableMap<String,​Path> extraOutputs,        com.google.common.collect.ImmutableList<Arg> args,        Optional<LinkOutputPostprocessor> postprocessor,        Optional<RuleScheduleInfo> ruleScheduleInfo,        boolean cacheable,        boolean thinLto,        boolean fatLto)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `java.util.stre       | `getAp                |                       |
        | am.Stream<BuildRule>` | pleDebugSymbolDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getArgs()`           |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Linker`              | `getLinker()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getLinkerMapPath()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleScheduleInfo`    | `g                    |                       |
        |                       | etRuleScheduleInfo()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getSou               | ::: block             |
        |                       | rcePathToSupplementar | Returns a SourcePath  |
        |                       | yOutput​(String name)` | to a named            |
        |                       |                       | supplementary output, |
        |                       |                       | or null if it does    |
        |                       |                       | not exist.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`B                   |
        |                       |                       | uildRule`](../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString`

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.toolchain.linker.Linker,java.nio.file.Path,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,java.util.Optional,java.util.Optional,boolean,boolean,boolean)}

        -   #### CxxLink

                public CxxLink​(BuildTarget buildTarget,
                               ProjectFilesystem projectFilesystem,
                               SourcePathRuleFinder ruleFinder,
                               CellPathResolver cellResolver,
                               Linker linker,
                               Path output,
                               com.google.common.collect.ImmutableMap<String,​Path> extraOutputs,
                               com.google.common.collect.ImmutableList<Arg> args,
                               Optional<LinkOutputPostprocessor> postprocessor,
                               Optional<RuleScheduleInfo> ruleScheduleInfo,
                               boolean cacheable,
                               boolean thinLto,
                               boolean fatLto)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAppleDebugSymbolDeps()}

        -   #### getAppleDebugSymbolDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> getAppleDebugSymbolDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAppleDebugSymbolDeps` in
                interface `HasAppleDebugSymbolDeps`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<CxxLink.Impl>`

        []{#getSourcePathToSupplementaryOutput(java.lang.String)}

        -   #### getSourcePathToSupplementaryOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToSupplementaryOutput​(String name)
            ```

            ::: block
            [Description copied from
            interface: `HasSupplementaryOutputs`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a SourcePath to a named supplementary output, or
            null if it does not exist.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToSupplementaryOutput` in
                interface `HasSupplementaryOutputs`

        []{#getRuleScheduleInfo()}

        -   #### getRuleScheduleInfo

            ``` methodSignature
            public RuleScheduleInfo getRuleScheduleInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleScheduleInfo` in
                interface `OverrideScheduleRule`

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

        []{#getLinkerMapPath()}

        -   #### getLinkerMapPath

            ``` methodSignature
            public Optional<Path> getLinkerMapPath()
            ```

        []{#getLinker()}

        -   #### getLinker

            ``` methodSignature
            public Linker getLinker()
            ```

        []{#getArgs()}

        -   #### getArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Arg> getArgs()
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
