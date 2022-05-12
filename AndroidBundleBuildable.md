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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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

## Class AndroidBundleBuildable {#class-androidbundlebuildable .title title="Class AndroidBundleBuildable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBundleBuildable

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class AndroidBundleBuildable
        extends Object

    ::: block
    The class is responsible to create final bundle by taking individual
    module information and passing to `Config.Bundletool` through
    [`AabBuilderStep`](AabBuilderStep.html "class in com.facebook.buck.android").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                     Field                    Description
          --------------------------------------------------------------------- ------------------------ -------------
          `protected AndroidSdkLocation`                                        `androidSdkLocation`      
          `protected com.google.common.collect.ImmutableSortedSet<APKModule>`   `apkModules`              
          `protected BinaryType`                                                `binaryType`              
          `protected BuildTarget`                                               `buildTarget`             
          `protected Optional<SourcePath>`                                      `bundleConfigFilePath`    
          `protected com.facebook.buck.android.DexFilesInfo`                    `dexFilesInfo`            
          `protected ProjectFilesystem`                                         `filesystem`              
          `protected Tool`                                                      `javaRuntimeLauncher`     
          `protected SourcePath`                                                `keystorePath`            
          `protected ResourceFilesInfo`                                         `resourceFilesInfo`       
          `protected boolean`                                                   `useDynamicFeature`       

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                  Description
          ------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Step>`   `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`    
          `BuildTarget`                                     `getBuildTarget()`                                                                       
          `ProjectFilesystem`                               `getProjectFilesystem()`                                                                 

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

        []{#dexFilesInfo}

        -   #### dexFilesInfo

                protected final com.facebook.buck.android.DexFilesInfo dexFilesInfo

        []{#resourceFilesInfo}

        -   #### resourceFilesInfo

                protected final ResourceFilesInfo resourceFilesInfo

        []{#keystorePath}

        -   #### keystorePath

                protected final SourcePath keystorePath

        []{#apkModules}

        -   #### apkModules

                protected final com.google.common.collect.ImmutableSortedSet<APKModule> apkModules

        []{#javaRuntimeLauncher}

        -   #### javaRuntimeLauncher

                protected final Tool javaRuntimeLauncher

        []{#binaryType}

        -   #### binaryType

                protected final BinaryType binaryType

        []{#bundleConfigFilePath}

        -   #### bundleConfigFilePath

                protected final Optional<SourcePath> bundleConfigFilePath

        []{#filesystem}

        -   #### filesystem

                protected final ProjectFilesystem filesystem

        []{#buildTarget}

        -   #### buildTarget

                protected final BuildTarget buildTarget

        []{#androidSdkLocation}

        -   #### androidSdkLocation

                protected final AndroidSdkLocation androidSdkLocation

        []{#useDynamicFeature}

        -   #### useDynamicFeature

                protected final boolean useDynamicFeature
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            public ProjectFilesystem getProjectFilesystem()
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
