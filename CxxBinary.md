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

## Class CxxBinary {#class-cxxbinary .title title="Class CxxBinary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.cxx.CxxBinary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `HasRuntimeDeps`,
        `HasSupplementaryOutputs`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`, `BinaryBuildRule`,
        `HasAppleDebugSymbolDeps`, `NativeTestable`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CxxBinary
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements BinaryBuildRule, NativeTestable, HasRuntimeDeps, HasAppleDebugSymbolDeps, SupportsInputBasedRuleKey, HasSupplementaryOutputs
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CxxBinary​(BuildTarget buildTarget,          ProjectFilesystem projectFilesystem,          BuildRuleParams params,          CxxPlatform cxxPlatform,          BuildRule linkRule,          Tool executable,          Iterable<FrameworkPath> frameworks,          Iterable<BuildTarget> tests,          BuildTarget platformlessTarget,          boolean cacheable)`    

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
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPlatform`         | `getCxxPlatform()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `getLinkRule()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPrivateCxxP       | ::: block             |
        | CxxPreprocessorInput` | reprocessorInput​(CxxP | Return the            |
        |                       | latform cxxPlatform,  | [`CxxPreprocessorInpu |
        |                       |                       | t`](CxxPreprocessorIn |
        |                       |          ActionGraphB | put.html "class in co |
        |                       | uilder graphBuilder)` | m.facebook.buck.cxx") |
        |                       |                       | to expose private     |
        |                       |                       | headers of this rule. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
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
        | `boolean`             | `isTestedBy​(B         | ::: block             |
        |                       | uildTarget testRule)` | Return true if this   |
        |                       |                       | rule is tested by     |
        |                       |                       | `testTarget`, false   |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.toolchain.tool.Tool,java.lang.Iterable,java.lang.Iterable,com.facebook.buck.core.model.BuildTarget,boolean)}

        -   #### CxxBinary

                public CxxBinary​(BuildTarget buildTarget,
                                 ProjectFilesystem projectFilesystem,
                                 BuildRuleParams params,
                                 CxxPlatform cxxPlatform,
                                 BuildRule linkRule,
                                 Tool executable,
                                 Iterable<FrameworkPath> frameworks,
                                 Iterable<BuildTarget> tests,
                                 BuildTarget platformlessTarget,
                                 boolean cacheable)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExecutableCommand(com.facebook.buck.core.model.OutputLabel)}

        -   #### getExecutableCommand

            ``` methodSignature
            public Tool getExecutableCommand​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `BinaryBuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Command to execute the output of this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutableCommand` in interface `BinaryBuildRule`

            [Parameters:]{.paramLabel}
            :   `outputLabel` - associated with the executable

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getLinkRule()}

        -   #### getLinkRule

            ``` methodSignature
            public BuildRule getLinkRule()
            ```

        []{#isTestedBy(com.facebook.buck.core.model.BuildTarget)}

        -   #### isTestedBy

            ``` methodSignature
            public boolean isTestedBy​(BuildTarget testRule)
            ```

            ::: block
            [Description copied from
            interface: `NativeTestable`]{.descfrmTypeLabel}
            :::

            ::: block
            Return true if this rule is tested by `testTarget`, false
            otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isTestedBy` in interface `NativeTestable`

        []{#getPrivateCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPrivateCxxPreprocessorInput

            ``` methodSignature
            public CxxPreprocessorInput getPrivateCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                       ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `NativeTestable`]{.descfrmTypeLabel}
            :::

            ::: block
            Return the
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            to expose private headers of this rule. This is used to
            propagate private headers to the test testing this object.
            For convenience, tests can see private headers visible in
            the rule being tested.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrivateCxxPreprocessorInput` in
                interface `NativeTestable`

        []{#getAppleDebugSymbolDeps()}

        -   #### getAppleDebugSymbolDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> getAppleDebugSymbolDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAppleDebugSymbolDeps` in
                interface `HasAppleDebugSymbolDeps`

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

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            public CxxPlatform getCxxPlatform()
            ```

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
