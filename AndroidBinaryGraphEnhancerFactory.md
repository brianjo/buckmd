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

## Class AndroidBinaryGraphEnhancerFactory {#class-androidbinarygraphenhancerfactory .title title="Class AndroidBinaryGraphEnhancerFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBinaryGraphEnhancerFactory

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidBinaryGraphEnhancerFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                             Description
          --------------------------------------- -------------
          `AndroidBinaryGraphEnhancerFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AndroidBinaryGraphEnhancer`   `create​(ToolchainProvider toolchainProvider,       JavaBuckConfig javaBuckConfig,       AndroidBuckConfig androidBuckConfig,       CxxBuckConfig cxxBuckConfig,       DxConfig dxConfig,       ProGuardConfig proGuardConfig,       CellPathResolver cellPathResolver,       TargetGraph targetGraph,       BuildTarget buildTarget,       DependencyStack dependencyStack,       ProjectFilesystem projectFilesystem,       BuildRuleParams params,       ActionGraphBuilder graphBuilder,       FilterResourcesSteps.ResourceFilter resourceFilter,       com.facebook.buck.android.DexSplitMode dexSplitMode,       EnumSet<ExopackageMode> exopackageModes,       java.util.function.Supplier<com.google.common.collect.ImmutableSet<JavaLibrary>> rulesToExcludeFromDex,       AndroidGraphEnhancerArgs args,       boolean useProtoFormat,       JavaOptions javaOptions,       JavacFactory javacFactory,       ConfigurationRuleRegistry configurationRuleRegistry)`    

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

        []{#<init>()}

        -   #### AndroidBinaryGraphEnhancerFactory

                public AndroidBinaryGraphEnhancerFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.jvm.java.JavaBuckConfig,com.facebook.buck.android.AndroidBuckConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.android.DxConfig,com.facebook.buck.android.ProGuardConfig,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.android.FilterResourcesSteps.ResourceFilter,com.facebook.buck.android.DexSplitMode,java.util.EnumSet,java.util.function.Supplier,com.facebook.buck.android.AndroidGraphEnhancerArgs,boolean,com.facebook.buck.jvm.java.JavaOptions,com.facebook.buck.jvm.java.JavacFactory,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry)}

        -   #### create

            ``` methodSignature
            public AndroidBinaryGraphEnhancer create​(ToolchainProvider toolchainProvider,
                                                     JavaBuckConfig javaBuckConfig,
                                                     AndroidBuckConfig androidBuckConfig,
                                                     CxxBuckConfig cxxBuckConfig,
                                                     DxConfig dxConfig,
                                                     ProGuardConfig proGuardConfig,
                                                     CellPathResolver cellPathResolver,
                                                     TargetGraph targetGraph,
                                                     BuildTarget buildTarget,
                                                     DependencyStack dependencyStack,
                                                     ProjectFilesystem projectFilesystem,
                                                     BuildRuleParams params,
                                                     ActionGraphBuilder graphBuilder,
                                                     FilterResourcesSteps.ResourceFilter resourceFilter,
                                                     com.facebook.buck.android.DexSplitMode dexSplitMode,
                                                     EnumSet<ExopackageMode> exopackageModes,
                                                     java.util.function.Supplier<com.google.common.collect.ImmutableSet<JavaLibrary>> rulesToExcludeFromDex,
                                                     AndroidGraphEnhancerArgs args,
                                                     boolean useProtoFormat,
                                                     JavaOptions javaOptions,
                                                     JavacFactory javacFactory,
                                                     ConfigurationRuleRegistry configurationRuleRegistry)
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
