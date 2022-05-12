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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class ConfiguredCompilerFactory {#class-configuredcompilerfactory .title title="Class ConfiguredCompilerFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.ConfiguredCompilerFactory

::: description
-   

    Direct Known Subclasses:
    :   `GroovyConfiguredCompilerFactory`,
        `JavaConfiguredCompilerFactory`,
        `KotlinConfiguredCompilerFactory`,
        `ScalaConfiguredCompilerFactory`

    ------------------------------------------------------------------------

        public abstract class ConfiguredCompilerFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `ConfiguredCompilerFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                                                                                                                                                                                                                                                   Description
          --------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`                                        `addTargetDeps​(TargetConfiguration targetConfiguration,              com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,              com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)`    
          `abstract CompileToJarStepFactory`            `configure​(JvmLibraryArg args,          JavacOptions javacOptions,          ActionGraphBuilder actionGraphBuilder,          BuildRuleResolver buildRuleResolver,          TargetConfiguration targetConfiguration,          ToolchainProvider toolchainProvider)`         
          `AbiGenerationMode`                           `getAbiGenerationMode()`                                                                                                                                                                                                                                                  
          `abstract Optional<ExtraClasspathProvider>`   `getExtraClasspathProvider​(ToolchainProvider toolchainProvider,                          TargetConfiguration toolchainTargetConfiguration)`                                                                                                                               
          `void`                                        `getNonProvidedClasspathDeps​(TargetConfiguration targetConfiguration,                            java.util.function.Consumer<BuildTarget> depsConsumer)`                                                                                                                  
          `boolean`                                     `shouldCompileAgainstAbis()`                                                                                                                                                                                                                                              
          `boolean`                                     `shouldDesugarInterfaceMethods()`                                                                                                                                                                                                                                         
          `boolean`                                     `shouldGenerateSourceAbi()`                                                                                                                                                                                                                                               
          `boolean`                                     `shouldGenerateSourceOnlyAbi()`                                                                                                                                                                                                                                           
          `boolean`                                     `shouldMigrateToSourceOnlyAbi()`                                                                                                                                                                                                                                          
          `boolean`                                     `sourceAbiCopiesFromLibraryTargetOutput()`                                                                                                                                                                                                                                
          `boolean`                                     `trackClassUsage​(JavacOptions javacOptions)`                                                                                                                                                                                                                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### ConfiguredCompilerFactory

                public ConfiguredCompilerFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#configure(com.facebook.buck.jvm.java.JvmLibraryArg,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.toolchain.ToolchainProvider)}

        -   #### configure

            ``` methodSignature
            public abstract CompileToJarStepFactory configure​(@Nullable
                                                              JvmLibraryArg args,
                                                              JavacOptions javacOptions,
                                                              ActionGraphBuilder actionGraphBuilder,
                                                              BuildRuleResolver buildRuleResolver,
                                                              TargetConfiguration targetConfiguration,
                                                              ToolchainProvider toolchainProvider)
            ```

        []{#getExtraClasspathProvider(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getExtraClasspathProvider

            ``` methodSignature
            public abstract Optional<ExtraClasspathProvider> getExtraClasspathProvider​(ToolchainProvider toolchainProvider,
                                                                                       TargetConfiguration toolchainTargetConfiguration)
            ```

        []{#trackClassUsage(com.facebook.buck.jvm.java.JavacOptions)}

        -   #### trackClassUsage

            ``` methodSignature
            public boolean trackClassUsage​(JavacOptions javacOptions)
            ```

        []{#shouldDesugarInterfaceMethods()}

        -   #### shouldDesugarInterfaceMethods

            ``` methodSignature
            public boolean shouldDesugarInterfaceMethods()
            ```

        []{#shouldCompileAgainstAbis()}

        -   #### shouldCompileAgainstAbis

            ``` methodSignature
            public boolean shouldCompileAgainstAbis()
            ```

        []{#getAbiGenerationMode()}

        -   #### getAbiGenerationMode

            ``` methodSignature
            public AbiGenerationMode getAbiGenerationMode()
            ```

        []{#shouldGenerateSourceAbi()}

        -   #### shouldGenerateSourceAbi

            ``` methodSignature
            public boolean shouldGenerateSourceAbi()
            ```

        []{#shouldGenerateSourceOnlyAbi()}

        -   #### shouldGenerateSourceOnlyAbi

            ``` methodSignature
            public boolean shouldGenerateSourceOnlyAbi()
            ```

        []{#shouldMigrateToSourceOnlyAbi()}

        -   #### shouldMigrateToSourceOnlyAbi

            ``` methodSignature
            public boolean shouldMigrateToSourceOnlyAbi()
            ```

        []{#sourceAbiCopiesFromLibraryTargetOutput()}

        -   #### sourceAbiCopiesFromLibraryTargetOutput

            ``` methodSignature
            public boolean sourceAbiCopiesFromLibraryTargetOutput()
            ```

        []{#addTargetDeps(com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addTargetDeps

            ``` methodSignature
            public void addTargetDeps​(TargetConfiguration targetConfiguration,
                                      com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                      com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

        []{#getNonProvidedClasspathDeps(com.facebook.buck.core.model.TargetConfiguration,java.util.function.Consumer)}

        -   #### getNonProvidedClasspathDeps

            ``` methodSignature
            public void getNonProvidedClasspathDeps​(TargetConfiguration targetConfiguration,
                                                    java.util.function.Consumer<BuildTarget> depsConsumer)
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
