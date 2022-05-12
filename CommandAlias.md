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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class CommandAlias {#class-commandalias .title title="Class CommandAlias"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.NoopBuildRule](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.shell.CommandAlias

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasRuntimeDeps`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `BinaryBuildRule`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CommandAlias
        extends NoopBuildRule
        implements BinaryBuildRule, HasRuntimeDeps

    ::: block
    A
    [`BinaryBuildRule`](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
    that wraps other build rules, and can optionally add extra
    arguments, environment variables, or run different tools per host
    [`Platform`](../util/environment/Platform.html "enum in com.facebook.buck.util.environment").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `                     | ::: block             |
        |                       | CommandAlias.Unsuppor | Specific runtime      |
        |                       | tedPlatformException` | exception type that   |
        |                       |                       | is thrown when trying |
        |                       |                       | to run a tool via     |
        |                       |                       | [`Comma               |
        |                       |                       | ndAlias`](CommandAlia |
        |                       |                       | s.html "class in com. |
        |                       |                       | facebook.buck.shell") |
        |                       |                       | on a platform that    |
        |                       |                       | has not been          |
        |                       |                       | provided.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandAlias​(BuildTarget buildTarget,             ProjectFilesystem projectFilesystem,             Optional<BuildRule> genericDelegate,             com.google.common.collect.ImmutableSortedMap<Platform,​BuildRule> platformDelegates,             com.google.common.collect.ImmutableList<Arg> args,             com.google.common.collect.ImmutableSortedMap<String,​Arg> env,             Platform platform)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `inputBas             |                       |
        |                       | edRuleKeyIsEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedMap,com.facebook.buck.util.environment.Platform)}

        -   #### CommandAlias

                public CommandAlias​(BuildTarget buildTarget,
                                    ProjectFilesystem projectFilesystem,
                                    Optional<BuildRule> genericDelegate,
                                    com.google.common.collect.ImmutableSortedMap<Platform,​BuildRule> platformDelegates,
                                    com.google.common.collect.ImmutableList<Arg> args,
                                    com.google.common.collect.ImmutableSortedMap<String,​Arg> env,
                                    Platform platform)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#inputBasedRuleKeyIsEnabled()}

        -   #### inputBasedRuleKeyIsEnabled

            ``` methodSignature
            public boolean inputBasedRuleKeyIsEnabled()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `inputBasedRuleKeyIsEnabled` in
                interface `SupportsInputBasedRuleKey`

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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
