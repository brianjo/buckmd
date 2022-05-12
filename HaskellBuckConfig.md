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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellBuckConfig {#class-haskellbuckconfig .title title="Class HaskellBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class HaskellBuckConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `HaskellBuckConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                       Description
          ------------------------------------------------------------- ------------------------------------------------------------ -------------
          `Optional<ArchiveContents>`                                   `getArchiveContents​(String section)`                          
          `Optional<ToolProvider>`                                      `getCompiler​(String section)`                                 
          `Optional<com.google.common.collect.ImmutableList<String>>`   `getCompilerFlags​(String section)`                            
          `Integer`                                                     `getCompilerMajorVersion​(String section)`                     
          `String`                                                      `getCompilerSource​(String section)`                           
          `String`                                                      `getDefaultSection()`                                         
          `java.util.function.Supplier<Path>`                           `getGhciBinutils​(String section)`                             
          `java.util.function.Supplier<Path>`                           `getGhciCc​(String section)`                                   
          `java.util.function.Supplier<Path>`                           `getGhciCpp​(String section)`                                  
          `java.util.function.Supplier<Path>`                           `getGhciCxx​(String section)`                                  
          `java.util.function.Supplier<Path>`                           `getGhciGhc​(String section)`                                  
          `java.util.function.Supplier<Path>`                           `getGhciIServ​(String section)`                                
          `java.util.function.Supplier<Path>`                           `getGhciIServProf​(String section)`                            
          `java.util.function.Supplier<Path>`                           `getGhciIservScriptTemplate​(String section)`                  
          `java.util.function.Supplier<Path>`                           `getGhciLib​(String section)`                                  
          `java.util.function.Supplier<Path>`                           `getGhciPackager​(String section)`                             
          `java.util.function.Supplier<Path>`                           `getGhciScriptTemplate​(String section)`                       
          `Optional<ToolProvider>`                                      `getHaddock​(String section)`                                  
          `String`                                                      `getHaddockSource​(String section)`                            
          `Optional<ToolProvider>`                                      `getLinker​(String section)`                                   
          `Optional<com.google.common.collect.ImmutableList<String>>`   `getLinkerFlags​(String section)`                              
          `String`                                                      `getLinkerSource​(String section)`                             
          `Optional<? extends Linker.LinkableDepType>`                  `getLinkStyleForStubHeader​(String section)`                   
          `Optional<String>`                                            `getPackageNamePrefix​(String section)`                        
          `Optional<ToolProvider>`                                      `getPackager​(String section)`                                 
          `String`                                                      `getPackagerSource​(String section)`                           
          `String`                                                      `getSectionForPlatform​(UnresolvedCxxPlatform cxxPlatform)`    
          `boolean`                                                     `getShouldCacheLinks​(String section)`                         
          `boolean`                                                     `getShouldUseArgsfile​(String section)`                        
          `Optional<Boolean>`                                           `getShouldUsedOldBinaryOutputLocation​(String section)`        
          `boolean`                                                     `getSupportExposePackage​(String section)`                     

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

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### HaskellBuckConfig

                public HaskellBuckConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDefaultSection()}

        -   #### getDefaultSection

            ``` methodSignature
            public String getDefaultSection()
            ```

        []{#getSectionForPlatform(com.facebook.buck.cxx.toolchain.UnresolvedCxxPlatform)}

        -   #### getSectionForPlatform

            ``` methodSignature
            public String getSectionForPlatform​(UnresolvedCxxPlatform cxxPlatform)
            ```

        []{#getCompilerMajorVersion(java.lang.String)}

        -   #### getCompilerMajorVersion

            ``` methodSignature
            public Integer getCompilerMajorVersion​(String section)
            ```

        []{#getCompiler(java.lang.String)}

        -   #### getCompiler

            ``` methodSignature
            public Optional<ToolProvider> getCompiler​(String section)
            ```

        []{#getCompilerSource(java.lang.String)}

        -   #### getCompilerSource

            ``` methodSignature
            public String getCompilerSource​(String section)
            ```

        []{#getLinker(java.lang.String)}

        -   #### getLinker

            ``` methodSignature
            public Optional<ToolProvider> getLinker​(String section)
            ```

        []{#getLinkerSource(java.lang.String)}

        -   #### getLinkerSource

            ``` methodSignature
            public String getLinkerSource​(String section)
            ```

        []{#getPackager(java.lang.String)}

        -   #### getPackager

            ``` methodSignature
            public Optional<ToolProvider> getPackager​(String section)
            ```

        []{#getPackagerSource(java.lang.String)}

        -   #### getPackagerSource

            ``` methodSignature
            public String getPackagerSource​(String section)
            ```

        []{#getHaddock(java.lang.String)}

        -   #### getHaddock

            ``` methodSignature
            public Optional<ToolProvider> getHaddock​(String section)
            ```

        []{#getHaddockSource(java.lang.String)}

        -   #### getHaddockSource

            ``` methodSignature
            public String getHaddockSource​(String section)
            ```

        []{#getCompilerFlags(java.lang.String)}

        -   #### getCompilerFlags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCompilerFlags​(String section)
            ```

        []{#getLinkerFlags(java.lang.String)}

        -   #### getLinkerFlags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getLinkerFlags​(String section)
            ```

        []{#getShouldCacheLinks(java.lang.String)}

        -   #### getShouldCacheLinks

            ``` methodSignature
            public boolean getShouldCacheLinks​(String section)
            ```

        []{#getShouldUseArgsfile(java.lang.String)}

        -   #### getShouldUseArgsfile

            ``` methodSignature
            public boolean getShouldUseArgsfile​(String section)
            ```

        []{#getShouldUsedOldBinaryOutputLocation(java.lang.String)}

        -   #### getShouldUsedOldBinaryOutputLocation

            ``` methodSignature
            public Optional<Boolean> getShouldUsedOldBinaryOutputLocation​(String section)
            ```

        []{#getSupportExposePackage(java.lang.String)}

        -   #### getSupportExposePackage

            ``` methodSignature
            public boolean getSupportExposePackage​(String section)
            ```

        []{#getArchiveContents(java.lang.String)}

        -   #### getArchiveContents

            ``` methodSignature
            public Optional<ArchiveContents> getArchiveContents​(String section)
            ```

        []{#getPackageNamePrefix(java.lang.String)}

        -   #### getPackageNamePrefix

            ``` methodSignature
            public Optional<String> getPackageNamePrefix​(String section)
            ```

        []{#getGhciScriptTemplate(java.lang.String)}

        -   #### getGhciScriptTemplate

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciScriptTemplate​(String section)
            ```

        []{#getGhciIservScriptTemplate(java.lang.String)}

        -   #### getGhciIservScriptTemplate

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciIservScriptTemplate​(String section)
            ```

        []{#getGhciBinutils(java.lang.String)}

        -   #### getGhciBinutils

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciBinutils​(String section)
            ```

        []{#getGhciGhc(java.lang.String)}

        -   #### getGhciGhc

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciGhc​(String section)
            ```

        []{#getGhciIServ(java.lang.String)}

        -   #### getGhciIServ

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciIServ​(String section)
            ```

        []{#getGhciIServProf(java.lang.String)}

        -   #### getGhciIServProf

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciIServProf​(String section)
            ```

        []{#getGhciLib(java.lang.String)}

        -   #### getGhciLib

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciLib​(String section)
            ```

        []{#getGhciCxx(java.lang.String)}

        -   #### getGhciCxx

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciCxx​(String section)
            ```

        []{#getGhciCc(java.lang.String)}

        -   #### getGhciCc

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciCc​(String section)
            ```

        []{#getGhciCpp(java.lang.String)}

        -   #### getGhciCpp

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciCpp​(String section)
            ```

        []{#getGhciPackager(java.lang.String)}

        -   #### getGhciPackager

            ``` methodSignature
            public java.util.function.Supplier<Path> getGhciPackager​(String section)
            ```

        []{#getLinkStyleForStubHeader(java.lang.String)}

        -   #### getLinkStyleForStubHeader

            ``` methodSignature
            public Optional<? extends Linker.LinkableDepType> getLinkStyleForStubHeader​(String section)
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
