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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class NdkToolchainBuildRule {#class-ndktoolchainbuildrule .title title="Class NdkToolchainBuildRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.NoopBuildRule](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.android.NdkToolchainBuildRule

::: description
-   

    All Implemented Interfaces:
    :   `ProvidesNdkCxxPlatform`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class NdkToolchainBuildRule
        extends NoopBuildRule
        implements ProvidesNdkCxxPlatform

    ::: block
    This
    [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    is just a placeholder to hold the created
    [`NdkCxxPlatform`](toolchain/ndk/NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk").
    It\'s a
    [`NoopBuildRule`](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")
    with no build steps or outputs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                           Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `NdkToolchainBuildRule​(BuildTarget buildTarget,                      ProjectFilesystem projectFilesystem,                      SourcePathResolverAdapter pathResolver,                      ProvidesCxxPlatform cxxPlatformRule,                      Optional<SourcePath> sharedRuntimePath,                      NdkCxxRuntime cxxRuntime,                      Tool objdump,                      Optional<SourcePath> ndkRoot)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                               Description
          ------------------- ------------------------------------ -------------
          `NdkCxxPlatform`    `getNdkCxxPlatform​(Flavor flavor)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRule](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `getBuildDeps, getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.cxx.toolchain.ProvidesCxxPlatform,java.util.Optional,com.facebook.buck.android.toolchain.ndk.NdkCxxRuntime,com.facebook.buck.core.toolchain.tool.Tool,java.util.Optional)}

        -   #### NdkToolchainBuildRule

                public NdkToolchainBuildRule​(BuildTarget buildTarget,
                                             ProjectFilesystem projectFilesystem,
                                             SourcePathResolverAdapter pathResolver,
                                             ProvidesCxxPlatform cxxPlatformRule,
                                             Optional<SourcePath> sharedRuntimePath,
                                             NdkCxxRuntime cxxRuntime,
                                             Tool objdump,
                                             Optional<SourcePath> ndkRoot)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNdkCxxPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### getNdkCxxPlatform

            ``` methodSignature
            public NdkCxxPlatform getNdkCxxPlatform​(Flavor flavor)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNdkCxxPlatform` in
                interface `ProvidesNdkCxxPlatform`
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
