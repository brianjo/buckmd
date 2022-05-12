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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.impl](package-summary.html)
:::

## Class AndroidPlatformTargetProducer {#class-androidplatformtargetproducer .title title="Class AndroidPlatformTargetProducer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.impl.AndroidPlatformTargetProducer

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidPlatformTargetProducer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `AndroidPlatformTargetProducer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                                                                                                                                                                                                                                                                                                                                             Description
          -------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static AndroidPlatformTarget`   `getDefaultPlatformTarget​(ProjectFilesystem filesystem,                         AndroidBuildToolsLocation androidBuildToolsLocation,                         AndroidSdkLocation androidSdkLocation,                         Optional<java.util.function.Supplier<Tool>> aaptOverride,                         Optional<ToolProvider> aapt2Override,                         AdbToolchain platformToolsLocation)`    
          `static AndroidPlatformTarget`   `getTargetForId​(ProjectFilesystem filesystem,               String platformId,               AndroidBuildToolsLocation androidBuildToolsLocation,               AndroidSdkLocation androidSdkLocation,               Optional<java.util.function.Supplier<Tool>> aaptOverride,               Optional<ToolProvider> aapt2Override,               AdbToolchain adbToolchain)`                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### AndroidPlatformTargetProducer

                public AndroidPlatformTargetProducer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetForId(com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,com.facebook.buck.android.toolchain.AndroidBuildToolsLocation,com.facebook.buck.android.toolchain.AndroidSdkLocation,java.util.Optional,java.util.Optional,com.facebook.buck.android.toolchain.AdbToolchain)}

        -   #### getTargetForId

            ``` methodSignature
            public static AndroidPlatformTarget getTargetForId​(ProjectFilesystem filesystem,
                                                               String platformId,
                                                               AndroidBuildToolsLocation androidBuildToolsLocation,
                                                               AndroidSdkLocation androidSdkLocation,
                                                               Optional<java.util.function.Supplier<Tool>> aaptOverride,
                                                               Optional<ToolProvider> aapt2Override,
                                                               AdbToolchain adbToolchain)
            ```

            [Parameters:]{.paramLabel}
            :   `platformId` - for the platform, such as \"Google
                Inc.:Google APIs:16\"

        []{#getDefaultPlatformTarget(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.android.toolchain.AndroidBuildToolsLocation,com.facebook.buck.android.toolchain.AndroidSdkLocation,java.util.Optional,java.util.Optional,com.facebook.buck.android.toolchain.AdbToolchain)}

        -   #### getDefaultPlatformTarget

            ``` methodSignature
            public static AndroidPlatformTarget getDefaultPlatformTarget​(ProjectFilesystem filesystem,
                                                                         AndroidBuildToolsLocation androidBuildToolsLocation,
                                                                         AndroidSdkLocation androidSdkLocation,
                                                                         Optional<java.util.function.Supplier<Tool>> aaptOverride,
                                                                         Optional<ToolProvider> aapt2Override,
                                                                         AdbToolchain platformToolsLocation)
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
