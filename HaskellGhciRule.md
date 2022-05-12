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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellGhciRule {#class-haskellghcirule .title title="Class HaskellGhciRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.haskell.HaskellGhciRule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `BinaryBuildRule`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class HaskellGhciRule
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements BinaryBuildRule
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `                     |                       |
        | atic HaskellGhciRule` | from​(BuildTarget buil |                       |
        |                       | dTarget,     ProjectF |                       |
        |                       | ilesystem projectFile |                       |
        |                       | system,     BuildRule |                       |
        |                       | Params params,     So |                       |
        |                       | urcePathRuleFinder ru |                       |
        |                       | leFinder,     com.fac |                       |
        |                       | ebook.buck.features.h |                       |
        |                       | askell.HaskellSources |                       |
        |                       |  srcs,     com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableList<String> comp |                       |
        |                       | ilerFlags,     Option |                       |
        |                       | al<SourcePath> ghciBi |                       |
        |                       | nDep,     Optional<So |                       |
        |                       | urcePath> ghciInit,   |                       |
        |                       |    BuildRule omnibusS |                       |
        |                       | haredObject,     com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSortedMap<S |                       |
        |                       | tring,​SourcePath> sol |                       |
        |                       | ibs,     com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leSortedMap<String,​So |                       |
        |                       | urcePath> preloadLibs |                       |
        |                       | ,     com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | et<com.facebook.buck. |                       |
        |                       | features.haskell.Hask |                       |
        |                       | ellPackage> firstOrde |                       |
        |                       | rHaskellPackages,     |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableSet<co |                       |
        |                       | m.facebook.buck.featu |                       |
        |                       | res.haskell.HaskellPa |                       |
        |                       | ckage> haskellPackage |                       |
        |                       | s,     com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | Set<com.facebook.buck |                       |
        |                       | .features.haskell.Has |                       |
        |                       | kellPackage> prebuilt |                       |
        |                       | HaskellPackages,      |                       |
        |                       | boolean enableProfili |                       |
        |                       | ng,     com.facebook. |                       |
        |                       | buck.features.haskell |                       |
        |                       | .HaskellPlatform plat |                       |
        |                       | form,     com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleList<SourcePath> e |                       |
        |                       | xtraScriptTemplates)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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

        []{#from(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.features.haskell.HaskellSources,com.google.common.collect.ImmutableList,java.util.Optional,java.util.Optional,com.facebook.buck.core.rules.BuildRule,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,boolean,com.facebook.buck.features.haskell.HaskellPlatform,com.google.common.collect.ImmutableList)}

        -   #### from

            ``` methodSignature
            public static HaskellGhciRule from​(BuildTarget buildTarget,
                                               ProjectFilesystem projectFilesystem,
                                               BuildRuleParams params,
                                               SourcePathRuleFinder ruleFinder,
                                               com.facebook.buck.features.haskell.HaskellSources srcs,
                                               com.google.common.collect.ImmutableList<String> compilerFlags,
                                               Optional<SourcePath> ghciBinDep,
                                               Optional<SourcePath> ghciInit,
                                               BuildRule omnibusSharedObject,
                                               com.google.common.collect.ImmutableSortedMap<String,​SourcePath> solibs,
                                               com.google.common.collect.ImmutableSortedMap<String,​SourcePath> preloadLibs,
                                               com.google.common.collect.ImmutableSet<com.facebook.buck.features.haskell.HaskellPackage> firstOrderHaskellPackages,
                                               com.google.common.collect.ImmutableSet<com.facebook.buck.features.haskell.HaskellPackage> haskellPackages,
                                               com.google.common.collect.ImmutableSet<com.facebook.buck.features.haskell.HaskellPackage> prebuiltHaskellPackages,
                                               boolean enableProfiling,
                                               com.facebook.buck.features.haskell.HaskellPlatform platform,
                                               com.google.common.collect.ImmutableList<SourcePath> extraScriptTemplates)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

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
