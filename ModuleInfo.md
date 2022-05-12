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

## Class ModuleInfo {#class-moduleinfo .title title="Class ModuleInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.ModuleInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ModuleInfo
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `ModuleInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                                   Description
          ---------------------------------------------------------------- ---------------------------------------- -------------
          `abstract com.google.common.collect.ImmutableMap<Path,​String>`   `getAssetDirectories()`                   
          `abstract com.google.common.collect.ImmutableSet<Path>`          `getDexFile()`                            
          `abstract com.google.common.collect.ImmutableSet<Path>`          `getJarFilesThatMayContainResources()`    
          `abstract String`                                                `getModuleName()`                         
          `abstract com.google.common.collect.ImmutableSet<Path>`          `getNativeLibraryDirectories()`           
          `abstract Path`                                                  `getResourceApk()`                        
          `abstract com.google.common.collect.ImmutableSet<Path>`          `getZipFiles()`                           
          `boolean`                                                        `isBaseModule()`                          

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

        -   #### ModuleInfo

                public ModuleInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getModuleName()}

        -   #### getModuleName

            ``` methodSignature
            @Parameter
            public abstract String getModuleName()
            ```

        []{#getResourceApk()}

        -   #### getResourceApk

            ``` methodSignature
            @Parameter
            @Nullable
            public abstract Path getResourceApk()
            ```

        []{#getDexFile()}

        -   #### getDexFile

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<Path> getDexFile()
            ```

        []{#getAssetDirectories()}

        -   #### getAssetDirectories

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableMap<Path,​String> getAssetDirectories()
            ```

        []{#getNativeLibraryDirectories()}

        -   #### getNativeLibraryDirectories

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<Path> getNativeLibraryDirectories()
            ```

        []{#getZipFiles()}

        -   #### getZipFiles

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<Path> getZipFiles()
            ```

        []{#getJarFilesThatMayContainResources()}

        -   #### getJarFilesThatMayContainResources

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<Path> getJarFilesThatMayContainResources()
            ```

        []{#isBaseModule()}

        -   #### isBaseModule

            ``` methodSignature
            public boolean isBaseModule()
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
