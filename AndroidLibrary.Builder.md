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

## Class AndroidLibrary.Builder {#class-androidlibrary.builder .title title="Class AndroidLibrary.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidLibrary.Builder

::: description
-   

    Enclosing class:
    :   [AndroidLibrary](AndroidLibrary.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static class AndroidLibrary.Builder
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                    Description
          -------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `Builder​(BuildTarget buildTarget,        ProjectFilesystem projectFilesystem,        ToolchainProvider toolchainProvider,        BuildRuleParams params,        ActionGraphBuilder graphBuilder,        JavaBuckConfig javaBuckConfig,        JavacFactory javacFactory,        JavacOptions javacOptions,        AndroidLibraryDescription.CoreArg args,        ConfiguredCompilerFactory compilerFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                   Description
          --------------------------- ------------------------ -------------
          `AndroidLibrary`            `build()`                 
          `BuildRule`                 `buildAbi()`              
          `DummyRDotJava`             `buildDummyRDotJava()`    
          `Optional<DummyRDotJava>`   `getDummyRDotJava()`      

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.jvm.java.JavaBuckConfig,com.facebook.buck.jvm.java.JavacFactory,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.android.AndroidLibraryDescription.CoreArg,com.facebook.buck.jvm.java.ConfiguredCompilerFactory)}

        -   #### Builder

                protected Builder​(BuildTarget buildTarget,
                                  ProjectFilesystem projectFilesystem,
                                  ToolchainProvider toolchainProvider,
                                  BuildRuleParams params,
                                  ActionGraphBuilder graphBuilder,
                                  JavaBuckConfig javaBuckConfig,
                                  JavacFactory javacFactory,
                                  JavacOptions javacOptions,
                                  AndroidLibraryDescription.CoreArg args,
                                  ConfiguredCompilerFactory compilerFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidLibrary build()
            ```

        []{#buildAbi()}

        -   #### buildAbi

            ``` methodSignature
            public BuildRule buildAbi()
            ```

        []{#buildDummyRDotJava()}

        -   #### buildDummyRDotJava

            ``` methodSignature
            public DummyRDotJava buildDummyRDotJava()
            ```

        []{#getDummyRDotJava()}

        -   #### getDummyRDotJava

            ``` methodSignature
            public Optional<DummyRDotJava> getDummyRDotJava()
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
