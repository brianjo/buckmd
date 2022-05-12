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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class BaseGenrule\<T extends [GenruleBuildable](GenruleBuildable.html "class in com.facebook.buck.shell")\> {#class-basegenrulet-extends-genrulebuildable .title title="Class BaseGenrule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   com.facebook.buck.shell.BaseGenrule\<T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - Buildable instance for the Genrule implementation.

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasOutputName`,
        `AllowsNonAnnotatedFields`, `HasMultipleOutputs`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ApkGenrule`, `ExternallyBuiltApplePackage`, `Genrule`,
        `JarGenrule`, `JsBundleGenrule`

    ------------------------------------------------------------------------

        public abstract class BaseGenrule<T extends GenruleBuildable>
        extends ModernBuildRule<T>
        implements HasOutputName, HasMultipleOutputs

    ::: block
    Abstract parent class of all Genrules, containing some common
    functionality while remaining generic over the
    [`Buildable`](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"),
    to be provided by child classes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                      Description
          -------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `BaseGenrule​(BuildTarget buildTarget,            ProjectFilesystem projectFilesystem,            BuildRuleResolver buildRuleResolver,            T buildable)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google           | `getOutputLabels()`   | ::: block             |
        | .common.collect.Immut |                       | returns a set of      |
        | ableSet<OutputLabel>` |                       | [`O                   |
        |                       |                       | utputLabel`](../core/ |
        |                       |                       | model/OutputLabel.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | instances associated  |
        |                       |                       | with this build rule. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getOutputName​(Outp   | ::: block             |
        |                       | utLabel outputLabel)` | Get the output name   |
        |                       |                       | of the generated      |
        |                       |                       | file, as listed in    |
        |                       |                       | the BUCK file.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  | ::: block             |
        |                       | SourcePathToOutput()` | Returns the output    |
        |                       |                       | defined in \'out\'.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSo                | ::: block             |
        | on.collect.ImmutableS | urcePathToOutput​(Outp | Returns               |
        | ortedSet<SourcePath>` | utLabel outputLabel)` | [`SourcePath`](       |
        |                       |                       | ../core/sourcepath/So |
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
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Get whether or not    |
        |                       |                       | the output of this    |
        |                       |                       | genrule can be        |
        |                       |                       | cached.               |
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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, hasBuildSteps, hashCode, injectFields, toString`

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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.shell.GenruleBuildable)}
        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,T)}

        -   #### BaseGenrule

                protected BaseGenrule​(BuildTarget buildTarget,
                                      ProjectFilesystem projectFilesystem,
                                      BuildRuleResolver buildRuleResolver,
                                      T buildable)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            ::: block
            Returns the output defined in \'out\'. Should not be used
            with multiple outputs. Use
            [`getSourcePathToOutput(OutputLabel)`](#getSourcePathToOutput(com.facebook.buck.core.model.OutputLabel))
            instead.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                interface `HasMultipleOutputs`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<T extends GenruleBuildable>`

        []{#getSourcePathToOutput(com.facebook.buck.core.model.OutputLabel)}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSourcePathToOutput​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `HasMultipleOutputs`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances to the outputs associated with the given output
            label, or `null` if the output label does not exist. If the
            default output label is given, returns the default outputs
            associated with the rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                interface `HasMultipleOutputs`

        []{#getOutputLabels()}

        -   #### getOutputLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<OutputLabel> getOutputLabels()
            ```

            ::: block
            [Description copied from
            interface: `HasMultipleOutputs`]{.descfrmTypeLabel}
            :::

            ::: block
            returns a set of
            [`OutputLabel`](../core/model/OutputLabel.html "class in com.facebook.buck.core.model")
            instances associated with this build rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputLabels` in interface `HasMultipleOutputs`

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getType` in class `AbstractBuildRule`

        []{#getOutputName(com.facebook.buck.core.model.OutputLabel)}

        -   #### getOutputName

            ``` methodSignature
            public String getOutputName​(OutputLabel outputLabel)
            ```

            ::: block
            Get the output name of the generated file, as listed in the
            BUCK file.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputName` in interface `HasOutputName`

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public final boolean isCacheable()
            ```

            ::: block
            Get whether or not the output of this genrule can be cached.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`
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
