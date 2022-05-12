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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Class NdkCxxPlatformTargetConfiguration {#class-ndkcxxplatformtargetconfiguration .title title="Class NdkCxxPlatformTargetConfiguration"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.ndk.NdkCxxPlatformTargetConfiguration

::: description
-   

    ------------------------------------------------------------------------

        public abstract class NdkCxxPlatformTargetConfiguration
        extends Object

    ::: block
    A container for all configuration settings needed to define a build
    target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                             Description
          --------------------------------------- -------------
          `NdkCxxPlatformTargetConfiguration()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                                                                             Description
          --------------------------------------------------- -------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`   `getAssemblerFlags​(NdkCompilerType type)`                                                           
          `abstract NdkCxxPlatformCompiler`                   `getCompiler()`                                                                                     
          `com.google.common.collect.ImmutableList<String>`   `getCompilerFlags​(NdkCompilerType type)`                                                            
          `com.google.common.collect.ImmutableList<String>`   `getLinkerFlags​(NdkCompilerType type)`                                                              
          `abstract String`                                   `getTargetAppPlatform()`                                                                            
          `int`                                               `getTargetAppPlatformLevel()`                                                                       
          `NdkTargetArch`                                     `getTargetArch()`                                                                                   
          `NdkTargetArchAbi`                                  `getTargetArchAbi()`                                                                                
          `abstract TargetCpuType`                            `getTargetCpuType()`                                                                                
          `NdkToolchain`                                      `getToolchain()`                                                                                    
          `NdkToolchainTarget`                                `getToolchainTarget()`                                                                              
          `static NdkCxxPlatformTargetConfiguration`          `of​(TargetCpuType targetCpuType,   String targetAppPlatform,   NdkCxxPlatformCompiler compiler)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        -   #### NdkCxxPlatformTargetConfiguration

                public NdkCxxPlatformTargetConfiguration()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.android.toolchain.ndk.TargetCpuType,java.lang.String,com.facebook.buck.android.toolchain.ndk.NdkCxxPlatformCompiler)}

        -   #### of

            ``` methodSignature
            public static NdkCxxPlatformTargetConfiguration of​(TargetCpuType targetCpuType,
                                                               String targetAppPlatform,
                                                               NdkCxxPlatformCompiler compiler)
            ```

        []{#getTargetCpuType()}

        -   #### getTargetCpuType

            ``` methodSignature
            public abstract TargetCpuType getTargetCpuType()
            ```

        []{#getTargetAppPlatform()}

        -   #### getTargetAppPlatform

            ``` methodSignature
            public abstract String getTargetAppPlatform()
            ```

        []{#getTargetAppPlatformLevel()}

        -   #### getTargetAppPlatformLevel

            ``` methodSignature
            @Derived
            public int getTargetAppPlatformLevel()
            ```

        []{#getCompiler()}

        -   #### getCompiler

            ``` methodSignature
            public abstract NdkCxxPlatformCompiler getCompiler()
            ```

        []{#getToolchain()}

        -   #### getToolchain

            ``` methodSignature
            @Derived
            public NdkToolchain getToolchain()
            ```

        []{#getToolchainTarget()}

        -   #### getToolchainTarget

            ``` methodSignature
            @Derived
            public NdkToolchainTarget getToolchainTarget()
            ```

        []{#getTargetArch()}

        -   #### getTargetArch

            ``` methodSignature
            @Derived
            public NdkTargetArch getTargetArch()
            ```

        []{#getTargetArchAbi()}

        -   #### getTargetArchAbi

            ``` methodSignature
            @Derived
            public NdkTargetArchAbi getTargetArchAbi()
            ```

        []{#getAssemblerFlags(com.facebook.buck.android.toolchain.ndk.NdkCompilerType)}

        -   #### getAssemblerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getAssemblerFlags​(NdkCompilerType type)
            ```

        []{#getCompilerFlags(com.facebook.buck.android.toolchain.ndk.NdkCompilerType)}

        -   #### getCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCompilerFlags​(NdkCompilerType type)
            ```

        []{#getLinkerFlags(com.facebook.buck.android.toolchain.ndk.NdkCompilerType)}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getLinkerFlags​(NdkCompilerType type)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
