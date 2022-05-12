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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class DefaultJavaLibraryRules.Builder {#class-defaultjavalibraryrules.builder .title title="Class DefaultJavaLibraryRules.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder

    -   -   com.facebook.buck.jvm.java.DefaultJavaLibraryRules.Builder

::: description
-   

    Enclosing class:
    :   [DefaultJavaLibraryRules](DefaultJavaLibraryRules.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        @AccessibleFields
        public static class DefaultJavaLibraryRules.Builder
        extends com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder}

            ### Fields inherited from class com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder

            `actionGraphBuilder, args, classesToRemoveFromJar, configuredCompilerFactory, constructor, deps, initialBuildTarget, initialParams, javaBuckConfig, javacOptions, manifestFile, mavenCoords, postprocessClassesCommands, proguardConfig, projectFilesystem, resources, resourcesRoot, sourceOnlyAbisAllowed, srcs, tests, toolchainProvider, unusedDependenciesAction`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                     Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Builder​(BuildTarget initialBuildTarget,        ProjectFilesystem projectFilesystem,        ToolchainProvider toolchainProvider,        BuildRuleParams initialParams,        ActionGraphBuilder graphBuilder,        ConfiguredCompilerFactory configuredCompilerFactory,        JavaBuckConfig javaBuckConfig,        JavaLibraryDescription.CoreArg args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method        Description
          ------------------- ------------- -------------
          `JavaLibraryDeps`   `getDeps()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder}

            ### Methods inherited from class com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder

            `addAllPostprocessClassesCommands, addAllResources, addAllSrcs, addAllTests, addPostprocessClassesCommands, addPostprocessClassesCommands, addResources, addResources, addSrcs, addSrcs, addTests, addTests, build, from, setClassesToRemoveFromJar, setConstructor, setDeps, setJavacOptions, setManifestFile, setManifestFile, setMavenCoords, setMavenCoords, setPostprocessClassesCommands, setProguardConfig, setProguardConfig, setResources, setResourcesRoot, setResourcesRoot, setSourceOnlyAbisAllowed, setSrcs, setTests`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.jvm.java.ConfiguredCompilerFactory,com.facebook.buck.jvm.java.JavaBuckConfig,com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg)}

        -   #### Builder

                public Builder​(BuildTarget initialBuildTarget,
                               ProjectFilesystem projectFilesystem,
                               ToolchainProvider toolchainProvider,
                               BuildRuleParams initialParams,
                               ActionGraphBuilder graphBuilder,
                               ConfiguredCompilerFactory configuredCompilerFactory,
                               @Nullable
                               JavaBuckConfig javaBuckConfig,
                               @Nullable
                               JavaLibraryDescription.CoreArg args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            @Nullable
            public JavaLibraryDeps getDeps()
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
