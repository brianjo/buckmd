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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class HeaderSymlinkTreeWithHeaderMap {#class-headersymlinktreewithheadermap .title title="Class HeaderSymlinkTreeWithHeaderMap"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.SymlinkTree](../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.MappedSymlinkTree](../core/rules/impl/MappedSymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            -   -   [com.facebook.buck.cxx.toolchain.HeaderSymlinkTree](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain")

                -   -   com.facebook.buck.cxx.HeaderSymlinkTreeWithHeaderMap

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasRuntimeDeps`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public final class HeaderSymlinkTreeWithHeaderMap
        extends HeaderSymlinkTree
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.impl.SymlinkTree}

            ### Fields inherited from class com.facebook.buck.core.rules.impl.[SymlinkTree](../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `category, root, type`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static HeaderSyml    | `cr                   |                       |
        | inkTreeWithHeaderMap` | eate​(BuildTarget targ |                       |
        |                       | et,       ProjectFile |                       |
        |                       | system filesystem,    |                       |
        |                       |     Path root,        |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Pat |                       |
        |                       | h,​SourcePath> links)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getH                 |                       |
        | Optional<SourcePath>` | eaderMapSourcePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PathSourcePath`      | `ge                   | ::: block             |
        |                       | tIncludeSourcePath()` | Get path to use as an |
        |                       |                       | include path to get   |
        |                       |                       | access to the files   |
        |                       |                       | in the tree.          |
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

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.MappedSymlinkTree}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[MappedSymlinkTree](../core/rules/impl/MappedSymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `getLinks`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.SymlinkTree}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[SymlinkTree](../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `getBuildDeps, getResolvedSymlinks, getRoot, getRootSourcePath, getRuntimeDeps, getType, getVerifyStep, isCacheable, resolveDuplicateRelativePaths, shouldDeleteExistingSymlink`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### create

            ``` methodSignature
            public static HeaderSymlinkTreeWithHeaderMap create​(BuildTarget target,
                                                                ProjectFilesystem filesystem,
                                                                Path root,
                                                                com.google.common.collect.ImmutableMap<Path,​SourcePath> links)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in class `SymlinkTree`

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in class `SymlinkTree`

        []{#getIncludeSourcePath()}

        -   #### getIncludeSourcePath

            ``` methodSignature
            public PathSourcePath getIncludeSourcePath()
            ```

            ::: block
            [Description copied from
            class: `HeaderSymlinkTree`]{.descfrmTypeLabel}
            :::

            ::: block
            Get path to use as an include path to get access to the
            files in the tree.
            If
            [`HeaderSymlinkTree.getHeaderMapSourcePath()`](toolchain/HeaderSymlinkTree.html#getHeaderMapSourcePath())
            is present, then the path it returns needs to be passed as
            an include path as well and it has to be passed before the
            path returned from this method.

            This path should not be added to rulekeys as a SourcePath
            (in some cases it points to the entire buck-out).
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getIncludeSourcePath` in class `HeaderSymlinkTree`

        []{#getHeaderMapSourcePath()}

        -   #### getHeaderMapSourcePath

            ``` methodSignature
            public Optional<SourcePath> getHeaderMapSourcePath()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getHeaderMapSourcePath` in class `HeaderSymlinkTree`
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
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
