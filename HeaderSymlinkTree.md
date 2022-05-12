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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class HeaderSymlinkTree {#class-headersymlinktree .title title="Class HeaderSymlinkTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.SymlinkTree](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.MappedSymlinkTree](../../core/rules/impl/MappedSymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.cxx.toolchain.HeaderSymlinkTree

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasRuntimeDeps`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `HeaderSymlinkTreeWithHeaderMap`,
        `HeaderSymlinkTreeWithModuleMap`

    ------------------------------------------------------------------------

        public class HeaderSymlinkTree
        extends MappedSymlinkTree
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

          Constructor                                                                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `HeaderSymlinkTree​(BuildTarget target,                  ProjectFilesystem filesystem,                  Path root,                  com.google.common.collect.ImmutableMap<Path,​SourcePath> links)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.MappedSymlinkTree}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[MappedSymlinkTree](../../core/rules/impl/MappedSymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `getLinks`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.SymlinkTree}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[SymlinkTree](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")

            `getBuildDeps, getBuildSteps, getResolvedSymlinks, getRoot, getRootSourcePath, getRuntimeDeps, getSourcePathToOutput, getType, getVerifyStep, isCacheable, resolveDuplicateRelativePaths, shouldDeleteExistingSymlink`

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### HeaderSymlinkTree

                public HeaderSymlinkTree​(BuildTarget target,
                                         ProjectFilesystem filesystem,
                                         Path root,
                                         com.google.common.collect.ImmutableMap<Path,​SourcePath> links)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludeSourcePath()}

        -   #### getIncludeSourcePath

            ``` methodSignature
            public PathSourcePath getIncludeSourcePath()
            ```

            ::: block
            Get path to use as an include path to get access to the
            files in the tree.
            If [`getHeaderMapSourcePath()`](#getHeaderMapSourcePath())
            is present, then the path it returns needs to be passed as
            an include path as well and it has to be passed before the
            path returned from this method.

            This path should not be added to rulekeys as a SourcePath
            (in some cases it points to the entire buck-out).
            :::

        []{#getHeaderMapSourcePath()}

        -   #### getHeaderMapSourcePath

            ``` methodSignature
            public Optional<SourcePath> getHeaderMapSourcePath()
            ```
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
