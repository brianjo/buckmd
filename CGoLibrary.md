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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Class CGoLibrary {#class-cgolibrary .title title="Class CGoLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.features.go.CGoLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CGoLibrary
        extends NoopBuildRuleWithDeclaredAndExtraDeps

    ::: block
    The CGoLibrary represents cgo build process which outputs the
    linkable object that is appended to the native go compiled program
    (via pack tool).
    The process consists of four steps (similiar to go build): 1.
    Generate c sources with cgo tool 2. Compile and link cgo sources
    into single object 3. Generate cgo_import.go 4. Return generated go
    files and linked object (used by GoCompile)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static BuildRule`    | `cre                  |                       |
        |                       | ate​(BuildRuleParams p |                       |
        |                       | arams,       BuildTar |                       |
        |                       | get buildTarget,      |                       |
        |                       |   ProjectFilesystem p |                       |
        |                       | rojectFilesystem,     |                       |
        |                       |    ActionGraphBuilder |                       |
        |                       |  graphBuilder,        |                       |
        |                       | CellPathResolver cell |                       |
        |                       | Roots,       CxxBuckC |                       |
        |                       | onfig cxxBuckConfig,  |                       |
        |                       |       com.facebook.bu |                       |
        |                       | ck.features.go.GoPlat |                       |
        |                       | form platform,        |                       |
        |                       | CgoLibraryDescription |                       |
        |                       | Arg args,       Itera |                       |
        |                       | ble<BuildTarget> cxxD |                       |
        |                       | eps,       Tool cgo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `ge                   | ::: block             |
        | .common.collect.Immut | tGeneratedGoSource()` | returns .go files     |
        | ableList<SourcePath>` |                       | produced by cgo tool  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `getLinkableDeps()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getOutput()`         | ::: block             |
        |                       |                       | returns compiled      |
        |                       |                       | linkable file source  |
        |                       |                       | path                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.features.go.GoPlatform,com.facebook.buck.features.go.CgoLibraryDescriptionArg,java.lang.Iterable,com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### create

            ``` methodSignature
            public static BuildRule create​(BuildRuleParams params,
                                           BuildTarget buildTarget,
                                           ProjectFilesystem projectFilesystem,
                                           ActionGraphBuilder graphBuilder,
                                           CellPathResolver cellRoots,
                                           CxxBuckConfig cxxBuckConfig,
                                           com.facebook.buck.features.go.GoPlatform platform,
                                           CgoLibraryDescriptionArg args,
                                           Iterable<BuildTarget> cxxDeps,
                                           Tool cgo)
            ```

        []{#getGeneratedGoSource()}

        -   #### getGeneratedGoSource

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getGeneratedGoSource()
            ```

            ::: block
            returns .go files produced by cgo tool
            :::

        []{#getOutput()}

        -   #### getOutput

            ``` methodSignature
            public SourcePath getOutput()
            ```

            ::: block
            returns compiled linkable file source path
            :::

        []{#getLinkableDeps()}

        -   #### getLinkableDeps

            ``` methodSignature
            public Iterable<BuildRule> getLinkableDeps()
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
