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
[Package]{.packageLabelInType} [com.facebook.buck.features.lua](package-summary.html)
:::

## Class LuaPlatform {#class-luaplatform .title title="Class LuaPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.lua.LuaPlatform

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`

    ------------------------------------------------------------------------

        public abstract class LuaPlatform
        extends Object
        implements FlavorConvertible
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type           Class                        Description
          --------------------------- ---------------------------- -------------
          `protected static class `   `LuaPlatform.PackageStyle`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                  Description
          ------------------- ---------------------- -------------
          `static String`     `FLAVOR_DOMAIN_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `LuaPlatform()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                                                                                    Description
          ------------------------------------------------------- --------------------------------------------------------------------------------------------------------- -------------
          `abstract CxxPlatform`                                  `getCxxPlatform()`                                                                                         
          `abstract String`                                       `getExtension()`                                                                                           
          `Flavor`                                                `getFlavor()`                                                                                              
          `abstract ToolProvider`                                 `getLua()`                                                                                                 
          `AbstractCxxLibraryGroup`                               `getLuaCxxLibrary​(BuildRuleResolver resolver,                 TargetConfiguration targetConfiguration)`    
          `abstract Optional<BuildTarget>`                        `getLuaCxxLibraryTarget()`                                                                                 
          `abstract NativeLinkStrategy`                           `getNativeLinkStrategy()`                                                                                  
          `abstract Optional<BuildTarget>`                        `getNativeStarterLibrary()`                                                                                
          `abstract ToolProvider`                                 `getPackager()`                                                                                            
          `abstract LuaPlatform.PackageStyle`                     `getPackageStyle()`                                                                                        
          `abstract Optional<LuaBinaryDescription.StarterType>`   `getStarterType()`                                                                                         
          `abstract boolean`                                      `shouldCacheBinaries()`                                                                                    
          `LuaPlatform`                                           `withExtension​(String extension)`                                                                          
          `LuaPlatform`                                           `withLua​(ToolProvider lua)`                                                                                
          `LuaPlatform`                                           `withNativeLinkStrategy​(NativeLinkStrategy nativeLinkStrategy)`                                            
          `LuaPlatform`                                           `withPackageStyle​(LuaPlatform.PackageStyle packageStyle)`                                                  

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
    -   []{#field.detail}

        ### Field Detail

        []{#FLAVOR_DOMAIN_NAME}

        -   #### FLAVOR_DOMAIN_NAME

                public static final String FLAVOR_DOMAIN_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.features.lua.LuaPlatform.FLAVOR_DOMAIN_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LuaPlatform

                public LuaPlatform()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#getLua()}

        -   #### getLua

            ``` methodSignature
            public abstract ToolProvider getLua()
            ```

        []{#getNativeStarterLibrary()}

        -   #### getNativeStarterLibrary

            ``` methodSignature
            public abstract Optional<BuildTarget> getNativeStarterLibrary()
            ```

        []{#getLuaCxxLibraryTarget()}

        -   #### getLuaCxxLibraryTarget

            ``` methodSignature
            public abstract Optional<BuildTarget> getLuaCxxLibraryTarget()
            ```

        []{#getStarterType()}

        -   #### getStarterType

            ``` methodSignature
            public abstract Optional<LuaBinaryDescription.StarterType> getStarterType()
            ```

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            public abstract String getExtension()
            ```

        []{#getPackageStyle()}

        -   #### getPackageStyle

            ``` methodSignature
            public abstract LuaPlatform.PackageStyle getPackageStyle()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`LuaPlatform.PackageStyle`](LuaPlatform.PackageStyle.html "enum in com.facebook.buck.features.lua")
                to use for Lua executables.

        []{#getPackager()}

        -   #### getPackager

            ``` methodSignature
            public abstract ToolProvider getPackager()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`ToolProvider`](../../core/toolchain/toolprovider/ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
                which packages standalone Lua executables.

        []{#shouldCacheBinaries()}

        -   #### shouldCacheBinaries

            ``` methodSignature
            public abstract boolean shouldCacheBinaries()
            ```

            [Returns:]{.returnLabel}
            :   whether to cache Lua executable packages.

        []{#getNativeLinkStrategy()}

        -   #### getNativeLinkStrategy

            ``` methodSignature
            public abstract NativeLinkStrategy getNativeLinkStrategy()
            ```

            [Returns:]{.returnLabel}
            :   the native link strategy to use for binaries.

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            public abstract CxxPlatform getCxxPlatform()
            ```

        []{#getLuaCxxLibrary(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getLuaCxxLibrary

            ``` methodSignature
            public AbstractCxxLibraryGroup getLuaCxxLibrary​(BuildRuleResolver resolver,
                                                            TargetConfiguration targetConfiguration)
            ```

        []{#withLua(com.facebook.buck.core.toolchain.toolprovider.ToolProvider)}

        -   #### withLua

            ``` methodSignature
            public LuaPlatform withLua​(ToolProvider lua)
            ```

        []{#withPackageStyle(com.facebook.buck.features.lua.LuaPlatform.PackageStyle)}

        -   #### withPackageStyle

            ``` methodSignature
            public LuaPlatform withPackageStyle​(LuaPlatform.PackageStyle packageStyle)
            ```

        []{#withNativeLinkStrategy(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkStrategy)}

        -   #### withNativeLinkStrategy

            ``` methodSignature
            public LuaPlatform withNativeLinkStrategy​(NativeLinkStrategy nativeLinkStrategy)
            ```

        []{#withExtension(java.lang.String)}

        -   #### withExtension

            ``` methodSignature
            public LuaPlatform withExtension​(String extension)
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
