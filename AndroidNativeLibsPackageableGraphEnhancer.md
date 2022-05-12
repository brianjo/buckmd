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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidNativeLibsPackageableGraphEnhancer {#class-androidnativelibspackageablegraphenhancer .title title="Class AndroidNativeLibsPackageableGraphEnhancer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidNativeLibsPackageableGraphEnhancer

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidNativeLibsPackageableGraphEnhancer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AndroidNativeLibsPackageableGraphEnhancer​(ToolchainProvider toolchainProvider,                                          CellPathResolver cellPathResolver,                                          ActionGraphBuilder graphBuilder,                                          BuildTarget originalBuildTarget,                                          ProjectFilesystem projectFilesystem,                                          com.google.common.collect.ImmutableSet<TargetCpuType> cpuFilters,                                          CxxBuckConfig cxxBuckConfig,                                          Optional<Map<String,​List<Pattern>>> nativeLibraryMergeMap,                                          Optional<BuildTarget> nativeLibraryMergeGlue,                                          Optional<com.google.common.collect.ImmutableSortedSet<String>> nativeLibraryMergeLocalizedSymbols,                                          com.facebook.buck.android.RelinkerMode relinkerMode,                                          com.google.common.collect.ImmutableList<Pattern> relinkerWhitelist,                                          APKModuleGraph apkModuleGraph,                                          AndroidNativeTargetConfigurationMatcher androidNativeTargetConfigurationMatcher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                               Method                                                          Description
          --------------------------------------------------------------------------------------------------------------- --------------------------------------------------------------- -------------
          `com.facebook.buck.android.AndroidNativeLibsPackageableGraphEnhancer.AndroidNativeLibsGraphEnhancementResult`   `enhance​(AndroidPackageableCollection packageableCollection)`    

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

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.config.CxxBuckConfig,java.util.Optional,java.util.Optional,java.util.Optional,com.facebook.buck.android.RelinkerMode,com.google.common.collect.ImmutableList,com.facebook.buck.android.apkmodule.APKModuleGraph,com.facebook.buck.android.AndroidNativeTargetConfigurationMatcher)}

        -   #### AndroidNativeLibsPackageableGraphEnhancer

                public AndroidNativeLibsPackageableGraphEnhancer​(ToolchainProvider toolchainProvider,
                                                                 CellPathResolver cellPathResolver,
                                                                 ActionGraphBuilder graphBuilder,
                                                                 BuildTarget originalBuildTarget,
                                                                 ProjectFilesystem projectFilesystem,
                                                                 com.google.common.collect.ImmutableSet<TargetCpuType> cpuFilters,
                                                                 CxxBuckConfig cxxBuckConfig,
                                                                 Optional<Map<String,​List<Pattern>>> nativeLibraryMergeMap,
                                                                 Optional<BuildTarget> nativeLibraryMergeGlue,
                                                                 Optional<com.google.common.collect.ImmutableSortedSet<String>> nativeLibraryMergeLocalizedSymbols,
                                                                 com.facebook.buck.android.RelinkerMode relinkerMode,
                                                                 com.google.common.collect.ImmutableList<Pattern> relinkerWhitelist,
                                                                 APKModuleGraph apkModuleGraph,
                                                                 AndroidNativeTargetConfigurationMatcher androidNativeTargetConfigurationMatcher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#enhance(com.facebook.buck.android.packageable.AndroidPackageableCollection)}

        -   #### enhance

            ``` methodSignature
            public com.facebook.buck.android.AndroidNativeLibsPackageableGraphEnhancer.AndroidNativeLibsGraphEnhancementResult enhance​(AndroidPackageableCollection packageableCollection)
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
