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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonBuckConfig {#class-pythonbuckconfig .title title="Class PythonBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class PythonBuckConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                             Description
          ------------------- --------------------------------- -------------
          `static class `     `PythonBuckConfig.PackageStyle`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                       Description
          ------------------- --------------------------- -------------
          `static Flavor`     `DEFAULT_PYTHON_PLATFORM`    
          `static String`     `SECTION`                    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                             Description
          --------------------------------------- -------------
          `PythonBuckConfig​(BuckConfig config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                                                                                Description
          --------------------------------------------------- ----------------------------------------------------------------------------------------------------- -------------
          `Flavor`                                            `calculatePythonPlatformFlavorFromSection​(String section)`                                             
          `Optional<String>`                                  `getConfiguredVersion​(String section)`                                                                 
          `Optional<BuildTarget>`                             `getCxxLibrary​(String section,              TargetConfiguration targetConfiguration)`                  
          `Flavor`                                            `getDefaultPythonPlatformFlavor()`                                                                     
          `String`                                            `getDefaultPythonPlatformSection()`                                                                    
          `String`                                            `getDefaultSection()`                                                                                  
          `BuckConfig`                                        `getDelegate()`                                                                                        
          `Optional<String>`                                  `getInterpreter​(String section)`                                                                       
          `NativeLinkStrategy`                                `getNativeLinkStrategy()`                                                                              
          `PythonBuckConfig.PackageStyle`                     `getPackageStyle()`                                                                                    
          `Optional<Tool>`                                    `getPexExecutor​(BuildRuleResolver resolver,               TargetConfiguration targetConfiguration)`    
          `Optional<BuildTarget>`                             `getPexExecutorTarget​(TargetConfiguration targetConfiguration)`                                        
          `String`                                            `getPexExtension()`                                                                                    
          `com.google.common.collect.ImmutableList<String>`   `getPexFlags()`                                                                                        
          `Optional<BuildTarget>`                             `getPexTarget​(TargetConfiguration targetConfiguration)`                                                
          `java.util.stream.Stream<String>`                   `getPythonPlatformSections()`                                                                          
          `Optional<Tool>`                                    `getRawPexTool​(BuildRuleResolver resolver,              TargetConfiguration targetConfiguration)`      
          `PathSourcePath`                                    `getSourcePath​(Path pythonPath)`                                                                       
          `com.google.common.collect.ImmutableList<String>`   `inplaceBinaryInterpreterFlags()`                                                                      
          `boolean`                                           `legacyOutputPath()`                                                                                   
          `boolean`                                           `shouldCacheBinaries()`                                                                                

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
    -   []{#field.detail}

        ### Field Detail

        []{#SECTION}

        -   #### SECTION

                public static final String SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.features.python.PythonBuckConfig.SECTION)

        []{#DEFAULT_PYTHON_PLATFORM}

        -   #### DEFAULT_PYTHON_PLATFORM

                public static final Flavor DEFAULT_PYTHON_PLATFORM
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### PythonBuckConfig

                public PythonBuckConfig​(BuckConfig config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

        []{#getInterpreter(java.lang.String)}

        -   #### getInterpreter

            ``` methodSignature
            public Optional<String> getInterpreter​(String section)
            ```

        []{#getPexTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getPexTarget

            ``` methodSignature
            public Optional<BuildTarget> getPexTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getPexFlags()}

        -   #### getPexFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPexFlags()
            ```

        []{#getRawPexTool(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRawPexTool

            ``` methodSignature
            public Optional<Tool> getRawPexTool​(BuildRuleResolver resolver,
                                                TargetConfiguration targetConfiguration)
            ```

        []{#getPexExecutorTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getPexExecutorTarget

            ``` methodSignature
            public Optional<BuildTarget> getPexExecutorTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getPexExecutor(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getPexExecutor

            ``` methodSignature
            public Optional<Tool> getPexExecutor​(BuildRuleResolver resolver,
                                                 TargetConfiguration targetConfiguration)
            ```

        []{#getNativeLinkStrategy()}

        -   #### getNativeLinkStrategy

            ``` methodSignature
            public NativeLinkStrategy getNativeLinkStrategy()
            ```

        []{#getPexExtension()}

        -   #### getPexExtension

            ``` methodSignature
            public String getPexExtension()
            ```

        []{#getConfiguredVersion(java.lang.String)}

        -   #### getConfiguredVersion

            ``` methodSignature
            public Optional<String> getConfiguredVersion​(String section)
            ```

        []{#shouldCacheBinaries()}

        -   #### shouldCacheBinaries

            ``` methodSignature
            public boolean shouldCacheBinaries()
            ```

        []{#legacyOutputPath()}

        -   #### legacyOutputPath

            ``` methodSignature
            public boolean legacyOutputPath()
            ```

        []{#getPackageStyle()}

        -   #### getPackageStyle

            ``` methodSignature
            public PythonBuckConfig.PackageStyle getPackageStyle()
            ```

        []{#inplaceBinaryInterpreterFlags()}

        -   #### inplaceBinaryInterpreterFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> inplaceBinaryInterpreterFlags()
            ```

            [Returns:]{.returnLabel}
            :   the flags that should be added to the hashbang of
                inplace python binaries

        []{#getDefaultPythonPlatformSection()}

        -   #### getDefaultPythonPlatformSection

            ``` methodSignature
            public String getDefaultPythonPlatformSection()
            ```

        []{#getDefaultPythonPlatformFlavor()}

        -   #### getDefaultPythonPlatformFlavor

            ``` methodSignature
            public Flavor getDefaultPythonPlatformFlavor()
            ```

        []{#getPythonPlatformSections()}

        -   #### getPythonPlatformSections

            ``` methodSignature
            public java.util.stream.Stream<String> getPythonPlatformSections()
            ```

        []{#calculatePythonPlatformFlavorFromSection(java.lang.String)}

        -   #### calculatePythonPlatformFlavorFromSection

            ``` methodSignature
            public Flavor calculatePythonPlatformFlavorFromSection​(String section)
            ```

        []{#getCxxLibrary(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getCxxLibrary

            ``` methodSignature
            public Optional<BuildTarget> getCxxLibrary​(String section,
                                                       TargetConfiguration targetConfiguration)
            ```

        []{#getDefaultSection()}

        -   #### getDefaultSection

            ``` methodSignature
            public String getDefaultSection()
            ```

        []{#getSourcePath(java.nio.file.Path)}

        -   #### getSourcePath

            ``` methodSignature
            public PathSourcePath getSourcePath​(Path pythonPath)
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
