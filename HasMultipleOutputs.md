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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface HasMultipleOutputs {#interface-hasmultipleoutputs .title title="Interface HasMultipleOutputs"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ApkGenrule`, `BaseGenrule`, `ExternallyBuiltApplePackage`,
        `Genrule`, `GenruleBinary`, `JarGenrule`, `JsBundleGenrule`,
        `RuleAnalysisLegacyBinaryBuildRuleView`,
        `RuleAnalysisLegacyBuildRuleView`,
        `RuleAnalysisLegacyTestBuildRuleView`

    ------------------------------------------------------------------------

        public interface HasMultipleOutputs
        extends BuildRule

    ::: block
    [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
    instances that support multiple outputs via output labels.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google           | `getOutputLabels()`   | ::: block             |
        | .common.collect.Immut |                       | returns a set of      |
        | ableSet<OutputLabel>` |                       | [                     |
        |                       |                       | `OutputLabel`](../../ |
        |                       |                       | model/OutputLabel.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | instances associated  |
        |                       |                       | with this build rule. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default SourcePath`  | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSo                | ::: block             |
        | on.collect.ImmutableS | urcePathToOutput​(Outp | Returns               |
        | ortedSet<SourcePath>` | utLabel outputLabel)` | [`SourcePath`         |
        |                       |                       | ](../../sourcepath/So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances to the      |
        |                       |                       | outputs associated    |
        |                       |                       | with the given output |
        |                       |                       | label, or `null` if   |
        |                       |                       | the output label does |
        |                       |                       | not exist.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePathToOutput(com.facebook.buck.core.model.OutputLabel)}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            com.google.common.collect.ImmutableSortedSet<SourcePath> getSourcePathToOutput​(OutputLabel outputLabel)
            ```

            ::: block
            Returns
            [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances to the outputs associated with the given output
            label, or `null` if the output label does not exist. If the
            default output label is given, returns the default outputs
            associated with the rule.
            :::

        []{#getOutputLabels()}

        -   #### getOutputLabels

            ``` methodSignature
            com.google.common.collect.ImmutableSet<OutputLabel> getOutputLabels()
            ```

            ::: block
            returns a set of
            [`OutputLabel`](../../model/OutputLabel.html "class in com.facebook.buck.core.model")
            instances associated with this build rule.
            :::

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            default SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
