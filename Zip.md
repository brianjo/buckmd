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
[Package]{.packageLabelInType} [com.facebook.buck.features.zip.rules](package-summary.html)
:::

## Class Zip {#class-zip .title title="Class Zip"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[Zip](Zip.html "class in com.facebook.buck.features.zip.rules")\>

        -   -   com.facebook.buck.features.zip.rules.Zip

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasOutputName`, `AddsToRuleKey`,
        `AllowsNonAnnotatedFields`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`, `Buildable`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class Zip
        extends ModernBuildRule<Zip>
        implements HasOutputName, Buildable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Zip​(SourcePathRuleFinder ruleFinder,    BuildTarget buildTarget,    ProjectFilesystem projectFilesystem,    String outputName,    com.google.common.collect.ImmutableSet<SourcePath> sources,    com.google.common.collect.ImmutableList<SourcePath> zipSources,    com.google.common.collect.ImmutableSet<Pattern> entriesToExclude,    OnDuplicateEntry onDuplicateEntry)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `getBuildSte          |                       |
        | google.common.collect | ps​(BuildContext build |                       |
        | .ImmutableList<Step>` | Context,              |                       |
        |                       |  ProjectFilesystem fi |                       |
        |                       | lesystem,             |                       |
        |                       |   OutputPathResolver  |                       |
        |                       | outputPathResolver,   |                       |
        |                       |             BuildCell |                       |
        |                       | RelativePathFactory b |                       |
        |                       | uildCellPathFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getOutputName​(Outp   | ::: block             |
        |                       | utLabel outputLabel)` | Returns an output     |
        |                       |                       | name for the build    |
        |                       |                       | target associated     |
        |                       |                       | with the given output |
        |                       |                       | label.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet,com.facebook.buck.util.zip.collect.OnDuplicateEntry)}

        -   #### Zip

                public Zip​(SourcePathRuleFinder ruleFinder,
                           BuildTarget buildTarget,
                           ProjectFilesystem projectFilesystem,
                           String outputName,
                           com.google.common.collect.ImmutableSet<SourcePath> sources,
                           com.google.common.collect.ImmutableList<SourcePath> zipSources,
                           com.google.common.collect.ImmutableSet<Pattern> entriesToExclude,
                           OnDuplicateEntry onDuplicateEntry)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                               ProjectFilesystem filesystem,
                                                                               OutputPathResolver outputPathResolver,
                                                                               BuildCellRelativePathFactory buildCellPathFactory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `Buildable`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in class `ModernBuildRule<Zip>`

        []{#getOutputName(com.facebook.buck.core.model.OutputLabel)}

        -   #### getOutputName

            ``` methodSignature
            public String getOutputName​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `HasOutputName`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an output name for the build target associated with
            the given output label. Not necessarily a path relative to
            any directory
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputName` in interface `HasOutputName`
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
