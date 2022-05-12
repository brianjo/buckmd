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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.impl](package-summary.html)
:::

## Class SymlinkTree {#class-symlinktree .title title="Class SymlinkTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.core.rules.impl.SymlinkTree

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
    :   `MappedSymlinkTree`, `PythonSymlinkTree`

    ------------------------------------------------------------------------

        public class SymlinkTree
        extends AbstractBuildRule
        implements HasRuntimeDeps, SupportsInputBasedRuleKey

    ::: block
    Creates a tree of symlinks inside of a given directory
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type    Field        Description
          -------------------- ------------ -------------
          `protected String`   `category`    
          `protected Path`     `root`        
          `protected String`   `type`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                              Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SymlinkTree​(String category,            BuildTarget target,            ProjectFilesystem filesystem,            SourcePathRuleFinder finder,            Path root,            Symlinks links)`           
          `SymlinkTree​(String category,            BuildTarget target,            ProjectFilesystem filesystem,            Path root,            com.google.common.collect.ImmutableMap<Path,​SourcePath> links)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pr                   | `getResolvedSym       |                       |
        | otected SymlinkPaths` | links​(SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getRootSourcePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Step`      | `getVerifyStep        |                       |
        |                       | ​(SymlinkPaths links)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildRule`]         |
        |                       |                       | (../BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `resolveDuplicateRe   | ::: block             |
        | atic com.google.commo | lativePaths​(com.googl | Because of            |
        | n.collect.ImmutableBi | e.common.collect.Immu | cross-cell, multiple  |
        | Map<SourcePath,​Path>` | tableSortedSet<Source | [`SourcePath`]        |
        |                       | Path> sourcePaths,    | (../../sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |       SourcePathResol | ce in com.facebook.bu |
        |                       | verAdapter resolver)` | ck.core.sourcepath")s |
        |                       |                       | can resolve to the    |
        |                       |                       | same relative path,   |
        |                       |                       | despite having        |
        |                       |                       | distinct absolute     |
        |                       |                       | paths.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `shouldDelete         |                       |
        |                       | ExistingSymlink​(Proje |                       |
        |                       | ctFilesystem filesyst |                       |
        |                       | em,                   |                       |
        |                       |           Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#category}

        -   #### category

                protected final String category

        []{#root}

        -   #### root

                protected final Path root

        []{#type}

        -   #### type

                protected final String type
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.nio.file.Path,com.facebook.buck.core.rules.impl.Symlinks)}

        -   #### SymlinkTree

                public SymlinkTree​(String category,
                                   BuildTarget target,
                                   ProjectFilesystem filesystem,
                                   SourcePathRuleFinder finder,
                                   Path root,
                                   Symlinks links)

        []{#<init>(java.lang.String,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### SymlinkTree

                public SymlinkTree​(String category,
                                   BuildTarget target,
                                   ProjectFilesystem filesystem,
                                   Path root,
                                   com.google.common.collect.ImmutableMap<Path,​SourcePath> links)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveDuplicateRelativePaths(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### resolveDuplicateRelativePaths

            ``` methodSignature
            public static com.google.common.collect.ImmutableBiMap<SourcePath,​Path> resolveDuplicateRelativePaths​(com.google.common.collect.ImmutableSortedSet<SourcePath> sourcePaths,
                                                                                                                        SourcePathResolverAdapter resolver)
            ```

            ::: block
            Because of cross-cell, multiple
            [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            can resolve to the same relative path, despite having
            distinct absolute paths. This presents a challenge for rules
            that require gathering all of the inputs in one directory.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcePaths` - set of SourcePaths to process

            [Returns:]{.returnLabel}
            :   a map that assigns a unique relative path to each of the
                SourcePaths.

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getType` in class `AbstractBuildRule`

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public SortedSet<BuildRule> getBuildDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `BuildRule`

            [Returns:]{.returnLabel}

            :   the set of rules that must be built before this rule.
                Normally, this matches the value of the `deps` argument
                for this build rule in the build file in which it was
                defined.

                However, there are special cases where other arguments
                pull in implicit dependencies (e.g., the `keystore`
                argument in `android_binary`). In these cases, the
                implicit dependencies are also included in the set
                returned by this method. The value of the original
                `deps` argument, as defined in the build file, must be
                accessed via a custom getter provided by the build rule.

        []{#getResolvedSymlinks(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getResolvedSymlinks

            ``` methodSignature
            protected SymlinkPaths getResolvedSymlinks​(SourcePathResolverAdapter resolver)
            ```

        []{#shouldDeleteExistingSymlink(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### shouldDeleteExistingSymlink

            ``` methodSignature
            protected boolean shouldDeleteExistingSymlink​(ProjectFilesystem filesystem,
                                                          Path path)
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getVerifyStep(com.facebook.buck.step.fs.SymlinkPaths)}

        -   #### getVerifyStep

            ``` methodSignature
            protected Step getVerifyStep​(SymlinkPaths links)
            ```

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            public Path getRoot()
            ```

        []{#getRootSourcePath()}

        -   #### getRootSourcePath

            ``` methodSignature
            public SourcePath getRootSourcePath()
            ```

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
