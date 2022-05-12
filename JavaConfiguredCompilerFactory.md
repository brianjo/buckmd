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

## Class JavaConfiguredCompilerFactory {#class-javaconfiguredcompilerfactory .title title="Class JavaConfiguredCompilerFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.jvm.java.ConfiguredCompilerFactory](ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")

    -   -   com.facebook.buck.jvm.java.JavaConfiguredCompilerFactory

::: description
-   

    ------------------------------------------------------------------------

        public class JavaConfiguredCompilerFactory
        extends ConfiguredCompilerFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                       Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaConfiguredCompilerFactory​(JavaBuckConfig javaBuckConfig,                              JavacFactory javacFactory)`                                                                                                                                                             
          `JavaConfiguredCompilerFactory​(JavaBuckConfig javaBuckConfig,                              java.util.function.BiFunction<ToolchainProvider,​TargetConfiguration,​ExtraClasspathProvider> extraClasspathProviderSupplier,                              JavacFactory javacFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                                                                                                                                                                                                                                             Description
          ------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CompileToJarStepFactory`            `configure​(JvmLibraryArg arg,          JavacOptions javacOptions,          ActionGraphBuilder actionGraphBuilder,          BuildRuleResolver buildRuleResolver,          TargetConfiguration targetConfiguration,          ToolchainProvider toolchainProvider)`    
          `AbiGenerationMode`                  `getAbiGenerationMode()`                                                                                                                                                                                                                                            
          `Optional<ExtraClasspathProvider>`   `getExtraClasspathProvider​(ToolchainProvider toolchainProvider,                          TargetConfiguration toolchainTargetConfiguration)`                                                                                                                         
          `boolean`                            `shouldCompileAgainstAbis()`                                                                                                                                                                                                                                        
          `boolean`                            `shouldDesugarInterfaceMethods()`                                                                                                                                                                                                                                   
          `boolean`                            `shouldGenerateSourceAbi()`                                                                                                                                                                                                                                         
          `boolean`                            `shouldGenerateSourceOnlyAbi()`                                                                                                                                                                                                                                     
          `boolean`                            `shouldMigrateToSourceOnlyAbi()`                                                                                                                                                                                                                                    
          `boolean`                            `trackClassUsage​(JavacOptions javacOptions)`                                                                                                                                                                                                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.ConfiguredCompilerFactory}

            ### Methods inherited from class com.facebook.buck.jvm.java.[ConfiguredCompilerFactory](ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")

            `addTargetDeps, getNonProvidedClasspathDeps, sourceAbiCopiesFromLibraryTargetOutput`

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

        []{#<init>(com.facebook.buck.jvm.java.JavaBuckConfig,com.facebook.buck.jvm.java.JavacFactory)}

        -   #### JavaConfiguredCompilerFactory

                public JavaConfiguredCompilerFactory​(JavaBuckConfig javaBuckConfig,
                                                     JavacFactory javacFactory)

        []{#<init>(com.facebook.buck.jvm.java.JavaBuckConfig,java.util.function.BiFunction,com.facebook.buck.jvm.java.JavacFactory)}

        -   #### JavaConfiguredCompilerFactory

                public JavaConfiguredCompilerFactory​(JavaBuckConfig javaBuckConfig,
                                                     java.util.function.BiFunction<ToolchainProvider,​TargetConfiguration,​ExtraClasspathProvider> extraClasspathProviderSupplier,
                                                     JavacFactory javacFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#trackClassUsage(com.facebook.buck.jvm.java.JavacOptions)}

        -   #### trackClassUsage

            ``` methodSignature
            public boolean trackClassUsage​(JavacOptions javacOptions)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `trackClassUsage` in class `ConfiguredCompilerFactory`

        []{#shouldDesugarInterfaceMethods()}

        -   #### shouldDesugarInterfaceMethods

            ``` methodSignature
            public boolean shouldDesugarInterfaceMethods()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldDesugarInterfaceMethods` in
                class `ConfiguredCompilerFactory`

        []{#shouldCompileAgainstAbis()}

        -   #### shouldCompileAgainstAbis

            ``` methodSignature
            public boolean shouldCompileAgainstAbis()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldCompileAgainstAbis` in
                class `ConfiguredCompilerFactory`

        []{#getAbiGenerationMode()}

        -   #### getAbiGenerationMode

            ``` methodSignature
            public AbiGenerationMode getAbiGenerationMode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getAbiGenerationMode` in
                class `ConfiguredCompilerFactory`

        []{#shouldGenerateSourceAbi()}

        -   #### shouldGenerateSourceAbi

            ``` methodSignature
            public boolean shouldGenerateSourceAbi()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldGenerateSourceAbi` in
                class `ConfiguredCompilerFactory`

        []{#shouldMigrateToSourceOnlyAbi()}

        -   #### shouldMigrateToSourceOnlyAbi

            ``` methodSignature
            public boolean shouldMigrateToSourceOnlyAbi()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldMigrateToSourceOnlyAbi` in
                class `ConfiguredCompilerFactory`

        []{#shouldGenerateSourceOnlyAbi()}

        -   #### shouldGenerateSourceOnlyAbi

            ``` methodSignature
            public boolean shouldGenerateSourceOnlyAbi()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldGenerateSourceOnlyAbi` in
                class `ConfiguredCompilerFactory`

        []{#configure(com.facebook.buck.jvm.java.JvmLibraryArg,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.toolchain.ToolchainProvider)}

        -   #### configure

            ``` methodSignature
            public CompileToJarStepFactory configure​(@Nullable
                                                     JvmLibraryArg arg,
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
