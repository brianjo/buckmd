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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain](package-summary.html)
:::

## Class AppleCxxPlatform {#class-applecxxplatform .title title="Class AppleCxxPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.AppleCxxPlatform

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`

    ------------------------------------------------------------------------

        public abstract class AppleCxxPlatform
        extends Object
        implements FlavorConvertible

    ::: block
    Adds Apple-specific tools to
    [`CxxPlatform`](../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                        Description
          ------------------- ---------------------------- -------------
          `static class `     `AppleCxxPlatform.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `AppleCxxPlatform()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                              Description
          ------------------------------------ --------------------------------------------------- -------------
          `static AppleCxxPlatform.Builder`    `builder()`                                          
          `abstract Tool`                      `getActool()`                                        
          `abstract AppleSdk`                  `getAppleSdk()`                                      
          `abstract AppleSdkPaths`             `getAppleSdkPaths()`                                 
          `abstract Optional<String>`          `getBuildVersion()`                                  
          `abstract Optional<Tool>`            `getCodesignAllocate()`                              
          `abstract ToolProvider`              `getCodesignProvider()`                              
          `abstract Optional<Tool>`            `getCopySceneKitAssets()`                            
          `abstract CxxPlatform`               `getCxxPlatform()`                                   
          `abstract Tool`                      `getDsymutil()`                                      
          `Flavor`                             `getFlavor()`                                        
          `abstract Tool`                      `getIbtool()`                                        
          `abstract Tool`                      `getLibtool()`                                       
          `abstract Tool`                      `getLipo()`                                          
          `abstract Tool`                      `getLldb()`                                          
          `abstract String`                    `getMinVersion()`                                    
          `abstract Tool`                      `getMomc()`                                          
          `abstract Optional<Path>`            `getStubBinary()`                                    
          `abstract Optional<SwiftPlatform>`   `getSwiftPlatform()`                                 
          `abstract Optional<String>`          `getXcodeBuildVersion()`                             
          `abstract Optional<String>`          `getXcodeVersion()`                                  
          `abstract Tool`                      `getXctest()`                                        
          `AppleCxxPlatform`                   `withAppleSdk​(AppleSdk appleSdk)`                    
          `AppleCxxPlatform`                   `withBuildVersion​(Optional<String> buildVersion)`    

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

        -   #### AppleCxxPlatform

                public AppleCxxPlatform()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            public abstract CxxPlatform getCxxPlatform()
            ```

        []{#getSwiftPlatform()}

        -   #### getSwiftPlatform

            ``` methodSignature
            public abstract Optional<SwiftPlatform> getSwiftPlatform()
            ```

        []{#getAppleSdk()}

        -   #### getAppleSdk

            ``` methodSignature
            public abstract AppleSdk getAppleSdk()
            ```

        []{#getAppleSdkPaths()}

        -   #### getAppleSdkPaths

            ``` methodSignature
            public abstract AppleSdkPaths getAppleSdkPaths()
            ```

        []{#getBuildVersion()}

        -   #### getBuildVersion

            ``` methodSignature
            public abstract Optional<String> getBuildVersion()
            ```

        []{#getMinVersion()}

        -   #### getMinVersion

            ``` methodSignature
            public abstract String getMinVersion()
            ```

        []{#getActool()}

        -   #### getActool

            ``` methodSignature
            public abstract Tool getActool()
            ```

        []{#getIbtool()}

        -   #### getIbtool

            ``` methodSignature
            public abstract Tool getIbtool()
            ```

        []{#getMomc()}

        -   #### getMomc

            ``` methodSignature
            public abstract Tool getMomc()
            ```

        []{#getCopySceneKitAssets()}

        -   #### getCopySceneKitAssets

            ``` methodSignature
            public abstract Optional<Tool> getCopySceneKitAssets()
            ```

        []{#getXctest()}

        -   #### getXctest

            ``` methodSignature
            public abstract Tool getXctest()
            ```

        []{#getDsymutil()}

        -   #### getDsymutil

            ``` methodSignature
            public abstract Tool getDsymutil()
            ```

        []{#getLibtool()}

        -   #### getLibtool

            ``` methodSignature
            public abstract Tool getLibtool()
            ```

        []{#getLipo()}

        -   #### getLipo

            ``` methodSignature
            public abstract Tool getLipo()
            ```

        []{#getStubBinary()}

        -   #### getStubBinary

            ``` methodSignature
            public abstract Optional<Path> getStubBinary()
            ```

        []{#getLldb()}

        -   #### getLldb

            ``` methodSignature
            public abstract Tool getLldb()
            ```

        []{#getCodesignProvider()}

        -   #### getCodesignProvider

            ``` methodSignature
            public abstract ToolProvider getCodesignProvider()
            ```

        []{#getCodesignAllocate()}

        -   #### getCodesignAllocate

            ``` methodSignature
            public abstract Optional<Tool> getCodesignAllocate()
            ```

        []{#getXcodeVersion()}

        -   #### getXcodeVersion

            ``` methodSignature
            public abstract Optional<String> getXcodeVersion()
            ```

        []{#getXcodeBuildVersion()}

        -   #### getXcodeBuildVersion

            ``` methodSignature
            public abstract Optional<String> getXcodeBuildVersion()
            ```

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleCxxPlatform.Builder builder()
            ```

        []{#withBuildVersion(java.util.Optional)}

        -   #### withBuildVersion

            ``` methodSignature
            public AppleCxxPlatform withBuildVersion​(Optional<String> buildVersion)
            ```

        []{#withAppleSdk(com.facebook.buck.apple.toolchain.AppleSdk)}

        -   #### withAppleSdk

            ``` methodSignature
            public AppleCxxPlatform withAppleSdk​(AppleSdk appleSdk)
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
