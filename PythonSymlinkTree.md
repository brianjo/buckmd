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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonSymlinkTree {#class-pythonsymlinktree .title title="Class PythonSymlinkTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.SymlinkTree](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.python.PythonSymlinkTree

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasRuntimeDeps`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PythonSymlinkTree
        extends SymlinkTree

    ::: block
    Creates a tree of symlinks inside of a given directory
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.impl.SymlinkTree}

            ### Fields inherited from class com.facebook.buck.core.rules.impl.[SymlinkTree](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `category, root, type`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `PythonSy                         | ::: block                         |
        | mlinkTree​(String category,        | Creates an instance of            |
        |            BuildTarget target,    | [                                 |
        |                ProjectFilesystem  | `SymlinkTree`](../../core/rules/i |
        | filesystem,                  Path | mpl/SymlinkTree.html "class in co |
        |  root,                  com.googl | m.facebook.buck.core.rules.impl") |
        | e.common.collect.ImmutableMap<Pat | :::                               |
        | h,​SourcePath> links,              |                                   |
        |      com.google.common.collect.Im |                                   |
        | mutableSortedSet<SourcePath> dire |                                   |
        | ctoriesToMerge,                   |                                   |
        | SourcePathRuleFinder ruleFinder)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                                                                                               Description
          --------------------- -------------------------------------------------------------------------------------------------------------------- -------------
          `protected boolean`   `shouldDeleteExistingSymlink​(ProjectFilesystem projectFilesystem,                            Path existingTarget)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.SymlinkTree}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[SymlinkTree](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `getBuildDeps, getBuildSteps, getResolvedSymlinks, getRoot, getRootSourcePath, getRuntimeDeps, getSourcePathToOutput, getType, getVerifyStep, isCacheable, resolveDuplicateRelativePaths`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### PythonSymlinkTree

                public PythonSymlinkTree​(String category,
                                         BuildTarget target,
                                         ProjectFilesystem filesystem,
                                         Path root,
                                         com.google.common.collect.ImmutableMap<Path,​SourcePath> links,
                                         com.google.common.collect.ImmutableSortedSet<SourcePath> directoriesToMerge,
                                         SourcePathRuleFinder ruleFinder)

            ::: block
            Creates an instance of
            [`SymlinkTree`](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
            :::

            [Parameters:]{.paramLabel}
            :   `category` - A name used in the symlink steps
            :   `target` - The target for this rule
            :   `filesystem` - The filesystem that the tree lives on
            :   `root` - The directory to create symlinks in
            :   `links` - A map of path within the link tree to the
                target of the symlikm
            :   `directoriesToMerge` - A map of relative paths within
                the link tree into which files from the value will be
                recursively linked. e.g. if a file at /tmp/foo/bar
                should be linked as /tmp/symlink-root/subdir/bar, the
                map should contain {Paths.get(\"subdir\"),
                SourcePath(Paths.get(\"tmp\", \"foo\")) }
            :   `ruleFinder` - Used to iterate over `directoriesToMerge`
                in order get the build time
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shouldDeleteExistingSymlink(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### shouldDeleteExistingSymlink

            ``` methodSignature
            protected boolean shouldDeleteExistingSymlink​(ProjectFilesystem projectFilesystem,
                                                          Path existingTarget)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldDeleteExistingSymlink` in class `SymlinkTree`
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
-   [Field](#field.summary) \| 
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
