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

## Class HaskellCompileRule {#class-haskellcompilerule .title title="Class HaskellCompileRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.haskell.HaskellCompileRule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class HaskellCompileRule
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `f                    |                       |
        | c HaskellCompileRule` | rom​(BuildTarget targe |                       |
        |                       | t,     ProjectFilesys |                       |
        |                       | tem projectFilesystem |                       |
        |                       | ,     BuildRuleParams |                       |
        |                       |  baseParams,     Sour |                       |
        |                       | cePathRuleFinder rule |                       |
        |                       | Finder,     Tool comp |                       |
        |                       | iler,     com.faceboo |                       |
        |                       | k.buck.features.haske |                       |
        |                       | ll.HaskellCompilerFla |                       |
        |                       | gs flags,     com.fac |                       |
        |                       | ebook.buck.features.h |                       |
        |                       | askell.HaskellPlatfor |                       |
        |                       | m platform,     Linke |                       |
        |                       | r.LinkableDepType dep |                       |
        |                       | Type,     boolean hsP |                       |
        |                       | rofile,     Optional< |                       |
        |                       | String> main,     Opt |                       |
        |                       | ional<com.facebook.bu |                       |
        |                       | ck.features.haskell.H |                       |
        |                       | askellPackageInfo> pa |                       |
        |                       | ckageInfo,     com.fa |                       |
        |                       | cebook.buck.features. |                       |
        |                       | haskell.HaskellSource |                       |
        |                       | s sources,     Prepro |                       |
        |                       | cessor preprocessor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getBu                |                       |
        | google.common.collect | ildSteps​(BuildContext |                       |
        | .ImmutableList<Step>` |  buildContext,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.go     | `getFlags()`          |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getInterfaces()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getModules()`        |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getObjects()`        |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getObjectsDir()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getStubsDir()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`Buil                |
        |                       |                       | dRule`](../../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.features.haskell.HaskellCompilerFlags,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,java.util.Optional,java.util.Optional,com.facebook.buck.features.haskell.HaskellSources,com.facebook.buck.cxx.toolchain.Preprocessor)}

        -   #### from

            ``` methodSignature
            public static HaskellCompileRule from​(BuildTarget target,
                                                  ProjectFilesystem projectFilesystem,
                                                  BuildRuleParams baseParams,
                                                  SourcePathRuleFinder ruleFinder,
                                                  Tool compiler,
                                                  com.facebook.buck.features.haskell.HaskellCompilerFlags flags,
                                                  com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                  Linker.LinkableDepType depType,
                                                  boolean hsProfile,
                                                  Optional<String> main,
                                                  Optional<com.facebook.buck.features.haskell.HaskellPackageInfo> packageInfo,
                                                  com.facebook.buck.features.haskell.HaskellSources sources,
                                                  Preprocessor preprocessor)
            ```

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                               BuildableContext buildableContext)
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
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

        []{#getObjects()}

        -   #### getObjects

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getObjects()
            ```

        []{#getModules()}

        -   #### getModules

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getModules()
            ```

        []{#getInterfaces()}

        -   #### getInterfaces

            ``` methodSignature
            public SourcePath getInterfaces()
            ```

        []{#getObjectsDir()}

        -   #### getObjectsDir

            ``` methodSignature
            public SourcePath getObjectsDir()
            ```

        []{#getStubsDir()}

        -   #### getStubsDir

            ``` methodSignature
            public SourcePath getStubsDir()
            ```

        []{#getFlags()}

        -   #### getFlags

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getFlags()
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
