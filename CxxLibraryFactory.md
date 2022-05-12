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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxLibraryFactory {#class-cxxlibraryfactory .title title="Class CxxLibraryFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxLibraryFactory

::: description
-   

    ------------------------------------------------------------------------

        public class CxxLibraryFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CxxLibraryFactory​(ToolchainProvider toolchainProvider,                  CxxBuckConfig cxxBuckConfig,                  InferBuckConfig inferBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               Description
          ------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildRule`               `createBuildRule​(TargetGraph targetGraph,                BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                BuildRuleParams metadataRuleParams,                ActionGraphBuilder graphBuilder,                CellPathResolver cellRoots,                CxxLibraryDescriptionArg args,                Optional<Linker.LinkableDepType> linkableDepType,                Optional<SourcePath> bundleLoader,                com.google.common.collect.ImmutableSet<BuildTarget> blacklist,                com.google.common.collect.ImmutableSortedSet<BuildTarget> extraDeps,                CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction transitiveCxxPreprocessorInputFunction,                CxxLibraryDescriptionDelegate delegate)`    
          `Iterable<BuildTarget>`   `getPlatformParseTimeDeps​(TargetConfiguration targetConfiguration)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.InferBuckConfig)}

        -   #### CxxLibraryFactory

                public CxxLibraryFactory​(ToolchainProvider toolchainProvider,
                                         CxxBuckConfig cxxBuckConfig,
                                         InferBuckConfig inferBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createBuildRule(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.CxxLibraryDescriptionArg,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.cxx.CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction,com.facebook.buck.cxx.CxxLibraryDescriptionDelegate)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(TargetGraph targetGraph,
                                             BuildTarget buildTarget,
                                             ProjectFilesystem projectFilesystem,
                                             BuildRuleParams metadataRuleParams,
                                             ActionGraphBuilder graphBuilder,
                                             CellPathResolver cellRoots,
                                             CxxLibraryDescriptionArg args,
                                             Optional<Linker.LinkableDepType> linkableDepType,
                                             Optional<SourcePath> bundleLoader,
                                             com.google.common.collect.ImmutableSet<BuildTarget> blacklist,
                                             com.google.common.collect.ImmutableSortedSet<BuildTarget> extraDeps,
                                             CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction transitiveCxxPreprocessorInputFunction,
                                             CxxLibraryDescriptionDelegate delegate)
            ```

        []{#getPlatformParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getPlatformParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getPlatformParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   an
                [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                with platform dependencies that need to be resolved at
                parse time.
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
