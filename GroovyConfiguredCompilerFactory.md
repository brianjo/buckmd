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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.groovy](package-summary.html)
:::

## Class GroovyConfiguredCompilerFactory {#class-groovyconfiguredcompilerfactory .title title="Class GroovyConfiguredCompilerFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.jvm.java.ConfiguredCompilerFactory](../java/ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")

    -   -   com.facebook.buck.jvm.groovy.GroovyConfiguredCompilerFactory

::: description
-   

    ------------------------------------------------------------------------

        public class GroovyConfiguredCompilerFactory
        extends ConfiguredCompilerFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `GroovyConfiguredCompilerFactory​(GroovyBuckConfig groovyBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                                                                                                                                                                                                                                                   Description
          ------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`                               `addTargetDeps​(TargetConfiguration targetConfiguration,              com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,              com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)`    
          `CompileToJarStepFactory`            `configure​(JvmLibraryArg args,          JavacOptions javacOptions,          ActionGraphBuilder actionGraphBuilder,          BuildRuleResolver buildRuleResolver,          TargetConfiguration targetConfiguration,          ToolchainProvider toolchainProvider)`         
          `Optional<ExtraClasspathProvider>`   `getExtraClasspathProvider​(ToolchainProvider toolchainProvider,                          TargetConfiguration toolchainTargetConfiguration)`                                                                                                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.ConfiguredCompilerFactory}

            ### Methods inherited from class com.facebook.buck.jvm.java.[ConfiguredCompilerFactory](../java/ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")

            `getAbiGenerationMode, getNonProvidedClasspathDeps, shouldCompileAgainstAbis, shouldDesugarInterfaceMethods, shouldGenerateSourceAbi, shouldGenerateSourceOnlyAbi, shouldMigrateToSourceOnlyAbi, sourceAbiCopiesFromLibraryTargetOutput, trackClassUsage`

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

        []{#<init>(com.facebook.buck.jvm.groovy.GroovyBuckConfig)}

        -   #### GroovyConfiguredCompilerFactory

                public GroovyConfiguredCompilerFactory​(GroovyBuckConfig groovyBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#configure(com.facebook.buck.jvm.java.JvmLibraryArg,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.toolchain.ToolchainProvider)}

        -   #### configure

            ``` methodSignature
            public CompileToJarStepFactory configure​(@Nullable
                                                     JvmLibraryArg args,
                                                     JavacOptions javacOptions,
                                                     ActionGraphBuilder actionGraphBuilder,
                                                     BuildRuleResolver buildRuleResolver,
                                                     TargetConfiguration targetConfiguration,
                                                     ToolchainProvider toolchainProvider)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `configure` in class `ConfiguredCompilerFactory`

        []{#getExtraClasspathProvider(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getExtraClasspathProvider

            ``` methodSignature
            public Optional<ExtraClasspathProvider> getExtraClasspathProvider​(ToolchainProvider toolchainProvider,
                                                                              TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraClasspathProvider` in
                class `ConfiguredCompilerFactory`

        []{#addTargetDeps(com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addTargetDeps

            ``` methodSignature
            public void addTargetDeps​(TargetConfiguration targetConfiguration,
                                      com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                      com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `addTargetDeps` in class `ConfiguredCompilerFactory`
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
