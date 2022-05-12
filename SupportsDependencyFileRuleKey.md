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

## Interface SupportsDependencyFileRuleKey {#interface-supportsdependencyfilerulekey .title title="Interface SupportsDependencyFileRuleKey"}
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
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `CalculateSourceAbi`,
        `CxxPreprocessAndCompile`, `DefaultJavaLibrary`

    ------------------------------------------------------------------------

        public interface SupportsDependencyFileRuleKey
        extends BuildRule

    ::: block
    Used to tag a rule that supports dependency-file input-based rule
    keys.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `java.util.function.P | `getCov               | ::: block             |
        | redicate<SourcePath>` | eredByDepFilePredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | a given path is       |
        |                       |                       | covered by dep-file   |
        |                       |                       | or not.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getExiste            | ::: block             |
        | redicate<SourcePath>` | nceOfInterestPredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | the existence of a    |
        |                       |                       | given path may be of  |
        |                       |                       | interest to compiler. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getInputsAf          | ::: block             |
        | .common.collect.Immut | terBuildingLocally​(Bu | Returns a list of     |
        | ableList<SourcePath>` | ildContext context,   | source paths that     |
        |                       |                       | were actually used    |
        |                       |        CellPathResolv | for the rule.         |
        |                       | er cellPathResolver)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useDepe              |                       |
        |                       | ndencyFileRuleKeys()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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

        []{#useDependencyFileRuleKeys()}

        -   #### useDependencyFileRuleKeys

            ``` methodSignature
            boolean useDependencyFileRuleKeys()
            ```

        []{#getCoveredByDepFilePredicate(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCoveredByDepFilePredicate

            ``` methodSignature
            java.util.function.Predicate<SourcePath> getCoveredByDepFilePredicate​(SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            Returns a predicate that can tell whether a given path is
            covered by dep-file or not. Note that being covered by
            dep-file doesn\'t necessarily mean being present in the
            dep-file. A covered path will only be present if actually
            used and that\'s the core idea of dep-file keys.
            I.e. this predicate should return true only for source paths
            that \*may\* be returned from
            [`getInputsAfterBuildingLocally(BuildContext, CellPathResolver)`](#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)).
            This information is used by the rule key builder to infer
            that inputs \*not\* in this list should be included
            unconditionally in the rule key. Inputs that \*are\* in this
            list should be included in the rule key if and only if they
            are actually being used for the rule. I.e. if they are
            present in the dep-file listed by
            [`getInputsAfterBuildingLocally(BuildContext, CellPathResolver)`](#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)).
            :::

        []{#getExistenceOfInterestPredicate(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getExistenceOfInterestPredicate

            ``` methodSignature
            java.util.function.Predicate<SourcePath> getExistenceOfInterestPredicate​(SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            Returns a predicate that can tell whether the existence of a
            given path may be of interest to compiler. If this predicate
            returns true, the path should be included in the rule key.
            Note that we only care about the existence here. The actual
            content of the file is not relevant.
            The main purpose of this predicate is to support scenarios
            where compiler decides whether to use a file or not solely
            based on its path. Of course, if compiler decides to use the
            file, it should list it in the dep-file in which case both
            the path and the content will be included in the rule key.
            However, relying only on presence in the dep-file for such
            paths is not sufficient. The problem occurs when a new such
            file just gets added, in which case it won\'t be present in
            the dep-file produced in the previous build, and yet if we
            run a local build now the compiler may decide to use it. For
            that reason rule key needs to reflect existence of all such
            files and change when a such a file gets added or removed.
            :::

        []{#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### getInputsAfterBuildingLocally

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getInputsAfterBuildingLocally​(BuildContext context,
                                                                                              CellPathResolver cellPathResolver)
                                                                                       throws IOException
            ```

            ::: block
            Returns a list of source paths that were actually used for
            the rule. This list comes from the dep-file produced by
            compiler.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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
