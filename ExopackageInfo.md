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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class ExopackageInfo {#class-exopackageinfo .title title="Class ExopackageInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.ExopackageInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ExopackageInfo
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                             Description
          --------------------- --------------------------------- -------------
          `static class `       `ExopackageInfo.Builder`           
          `static interface `   `ExopackageInfo.DexInfo`           
          `static interface `   `ExopackageInfo.NativeLibsInfo`    
          `static interface `   `ExopackageInfo.ResourcesInfo`     

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `ExopackageInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                      Method                  Description
          -------------------------------------------------------------------------------------- ----------------------- -------------
          `static ExopackageInfo.Builder`                                                        `builder()`              
          `protected void`                                                                       `check()`                
          `abstract Optional<ExopackageInfo.DexInfo>`                                            `getDexInfo()`           
          `abstract Optional<com.google.common.collect.ImmutableList<ExopackageInfo.DexInfo>>`   `getModuleInfo()`        
          `abstract Optional<ExopackageInfo.NativeLibsInfo>`                                     `getNativeLibsInfo()`    
          `java.util.stream.Stream<SourcePath>`                                                  `getRequiredPaths()`     
          `abstract Optional<ExopackageInfo.ResourcesInfo>`                                      `getResourcesInfo()`     

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

        -   #### ExopackageInfo

                public ExopackageInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDexInfo()}

        -   #### getDexInfo

            ``` methodSignature
            public abstract Optional<ExopackageInfo.DexInfo> getDexInfo()
            ```

        []{#getModuleInfo()}

        -   #### getModuleInfo

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableList<ExopackageInfo.DexInfo>> getModuleInfo()
            ```

        []{#getNativeLibsInfo()}

        -   #### getNativeLibsInfo

            ``` methodSignature
            public abstract Optional<ExopackageInfo.NativeLibsInfo> getNativeLibsInfo()
            ```

        []{#getResourcesInfo()}

        -   #### getResourcesInfo

            ``` methodSignature
            public abstract Optional<ExopackageInfo.ResourcesInfo> getResourcesInfo()
            ```

        []{#getRequiredPaths()}

        -   #### getRequiredPaths

            ``` methodSignature
            public java.util.stream.Stream<SourcePath> getRequiredPaths()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ExopackageInfo.Builder builder()
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
