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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleBundle {#class-applebundle .title title="Class AppleBundle"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.apple.AppleBundle

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleWithBinary`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasRuntimeDeps`, `BuildRule`,
        `HasNameAndType`, `BinaryBuildRule`, `NativeTestable`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AppleBundle
        extends AbstractBuildRule
        implements NativeTestable, BuildRuleWithBinary, HasRuntimeDeps, BinaryBuildRule

    ::: block
    Creates a bundle: a directory containing files and subdirectories,
    described by an Info.plist.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                      Description
          ------------------- -------------------------- -------------
          `static String`     `CODE_SIGN_ENTITLEMENTS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addSwi               | ::: block             |
        |                       | ftStdlibStepIfNeeded​( | A wrapper around      |
        |                       | SourcePathResolverAda | AppleRes              |
        |                       | pter resolver,        | ourceProcessing.addSw |
        |                       |                     P | iftStdlibStepIfNeeded |
        |                       | ath destinationPath,  | :::                   |
        |                       |                       |                       |
        |                       |      Optional<java.ut |                       |
        |                       | il.function.Supplier< |                       |
        |                       | CodeSignIdentity>> co |                       |
        |                       | deSignIdentitySupplie |                       |
        |                       | r,                    |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList.Builder<Step> s |                       |
        |                       | tepsBuilder,          |                       |
        |                       |                   boo |                       |
        |                       | lean isForPackaging)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<AppleDsym>` | `getAppleDsym()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildRule>` | `getBinary()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `                     |                       |
        |                       | getBinaryBuildRule()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getBinaryName​(Build  |                       |
        |                       | Target buildTarget,   |                       |
        |                       |             Optional< |                       |
        |                       | String> productName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getBundleRoot​(Proje  |                       |
        |                       | ctFilesystem filesyst |                       |
        |                       | em,              Buil |                       |
        |                       | dTarget buildTarget,  |                       |
        |                       |              String b |                       |
        |                       | inaryName,            |                       |
        |                       |    String extension)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getExtension()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getInfoPlistPath()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `getIsAppClip()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPlatformName()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPrivateCxxP       | ::: block             |
        | CxxPreprocessorInput` | reprocessorInput​(CxxP | Return the            |
        |                       | latform cxxPlatform,  | [`CxxPr               |
        |                       |                       | eprocessorInput`](../ |
        |                       |          ActionGraphB | cxx/CxxPreprocessorIn |
        |                       | uilder graphBuilder)` | put.html "class in co |
        |                       |                       | m.facebook.buck.cxx") |
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
        | `Path`                | `getUnzippedOutp      |                       |
        |                       | utFilePathToBinary()` |                       |
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
        | `boolean`             | `isLegacyWatchApp()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTestedBy​(B         | ::: block             |
        |                       | uildTarget testRule)` | Return true if this   |
        |                       |                       | rule is tested by     |
        |                       |                       | `testTarget`, false   |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateBuildRul       | ::: block             |
        |                       | eResolver​(BuildRuleRe | Updates the           |
        |                       | solver ruleResolver)` | BuildRuleResolver and |
        |                       |                       | associated objects    |
        |                       |                       | for this build rule.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `w                    |                       |
        | ommon.collect.Immutab | ithDefaults​(com.googl |                       |
        | leMap<String,​String>` | e.common.collect.Immu |                       |
        |                       | tableMap<String,​Strin |                       |
        |                       | g> map,             c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableMap<Stri |                       |
        |                       | ng,​String> defaults)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

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
    -   []{#field.detail}

        ### Field Detail

        []{#CODE_SIGN_ENTITLEMENTS}

        -   #### CODE_SIGN_ENTITLEMENTS

                public static final String CODE_SIGN_ENTITLEMENTS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.apple.AppleBundle.CODE_SIGN_ENTITLEMENTS)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBinaryName(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### getBinaryName

            ``` methodSignature
            public static String getBinaryName​(BuildTarget buildTarget,
                                               Optional<String> productName)
            ```

        []{#getBundleRoot(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String)}

        -   #### getBundleRoot

            ``` methodSignature
            public static Path getBundleRoot​(ProjectFilesystem filesystem,
                                             BuildTarget buildTarget,
                                             String binaryName,
                                             String extension)
            ```

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            public String getExtension()
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getInfoPlistPath()}

        -   #### getInfoPlistPath

            ``` methodSignature
            public Path getInfoPlistPath()
            ```

        []{#getUnzippedOutputFilePathToBinary()}

        -   #### getUnzippedOutputFilePathToBinary

            ``` methodSignature
            public Path getUnzippedOutputFilePathToBinary()
            ```

        []{#getPlatformName()}

        -   #### getPlatformName

            ``` methodSignature
            public String getPlatformName()
            ```

        []{#getBinary()}

        -   #### getBinary

            ``` methodSignature
            public Optional<BuildRule> getBinary()
            ```

        []{#getAppleDsym()}

        -   #### getAppleDsym

            ``` methodSignature
            public Optional<AppleDsym> getAppleDsym()
            ```

        []{#isLegacyWatchApp()}

        -   #### isLegacyWatchApp

            ``` methodSignature
            public boolean isLegacyWatchApp()
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#addSwiftStdlibStepIfNeeded(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,java.util.Optional,com.google.common.collect.ImmutableList.Builder,boolean)}

        -   #### addSwiftStdlibStepIfNeeded

            ``` methodSignature
            public void addSwiftStdlibStepIfNeeded​(SourcePathResolverAdapter resolver,
                                                   Path destinationPath,
                                                   Optional<java.util.function.Supplier<CodeSignIdentity>> codeSignIdentitySupplier,
                                                   com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                   boolean isForPackaging)
            ```

            ::: block
            A wrapper around
            AppleResourceProcessing.addSwiftStdlibStepIfNeeded
            :::

        []{#withDefaults(com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap)}

        -   #### withDefaults

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​String> withDefaults​(com.google.common.collect.ImmutableMap<String,​String> map,
                                                                                                   com.google.common.collect.ImmutableMap<String,​String> defaults)
            ```

        []{#getIsAppClip()}

        -   #### getIsAppClip

            ``` methodSignature
            public Boolean getIsAppClip()
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
            [`CxxPreprocessorInput`](../cxx/CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            to expose private headers of this rule. This is used to
            propagate private headers to the test testing this object.
            For convenience, tests can see private headers visible in
            the rule being tested.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrivateCxxPreprocessorInput` in
                interface `NativeTestable`

        []{#getBinaryBuildRule()}

        -   #### getBinaryBuildRule

            ``` methodSignature
            public BuildRule getBinaryBuildRule()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBinaryBuildRule` in interface `BuildRuleWithBinary`

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public SortedSet<BuildRule> getBuildDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `BuildRule`

            [Returns:]{.returnLabel}

            :   the set of rules that must be built before this rule.
                Normally, this matches the value of the `deps` argument
                for this build rule in the build file in which it was
                defined.

                However, there are special cases where other arguments
                pull in implicit dependencies (e.g., the `keystore`
                argument in `android_binary`). In these cases, the
                implicit dependencies are also included in the set
                returned by this method. The value of the original
                `deps` argument, as defined in the build file, must be
                accessed via a custom getter provided by the build rule.

        []{#updateBuildRuleResolver(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### updateBuildRuleResolver

            ``` methodSignature
            public void updateBuildRuleResolver​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Updates the BuildRuleResolver and associated objects for
            this build rule.
            Build rules sometimes hold field references to build rule
            resolvers. If this build rule is to be cached, it must
            update its BuildRuleResolver when a new action graph is
            constructed to avoid leaking the entire action graph it was
            originally associated with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in class `AbstractBuildRule`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
