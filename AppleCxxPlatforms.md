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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain.impl](package-summary.html)
:::

## Class AppleCxxPlatforms {#class-applecxxplatforms .title title="Class AppleCxxPlatforms"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.impl.AppleCxxPlatforms

::: description
-   

    ------------------------------------------------------------------------

        public class AppleCxxPlatforms
        extends Object

    ::: block
    Utility class to create Objective-C/C/C++/Objective-C++ platforms to
    support building iOS and Mac OS X products with Xcode.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                        Description
          ------------------- -------------------------------------------- -------------
          `static class `     `AppleCxxPlatforms.XcodeBuildVersionCache`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                    Method                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          -------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static com.google.common.collect.ImmutableList<AppleCxxPlatform>`   `buildAppleCxxPlatforms​(Optional<com.google.common.collect.ImmutableMap<AppleSdk,​AppleSdkPaths>> sdkPaths,                       Optional<com.google.common.collect.ImmutableMap<String,​AppleToolchain>> toolchains,                       ProjectFilesystem filesystem,                       BuckConfig buckConfig)`                                                                                                                                 
          `static AppleCxxPlatform`                                            `buildWithXcodeToolFinder​(ProjectFilesystem filesystem,                         AppleSdk targetSdk,                         String minVersion,                         String targetArchitecture,                         AppleSdkPaths sdkPaths,                         BuckConfig buckConfig,                         XcodeToolFinder xcodeToolFinder,                         AppleCxxPlatforms.XcodeBuildVersionCache xcodeBuildVersionCache)`    

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
    -   []{#method.detail}

        ### Method Detail

        []{#buildAppleCxxPlatforms(java.util.Optional,java.util.Optional,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.config.BuckConfig)}

        -   #### buildAppleCxxPlatforms

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<AppleCxxPlatform> buildAppleCxxPlatforms​(Optional<com.google.common.collect.ImmutableMap<AppleSdk,​AppleSdkPaths>> sdkPaths,
                                                                                                           Optional<com.google.common.collect.ImmutableMap<String,​AppleToolchain>> toolchains,
                                                                                                           ProjectFilesystem filesystem,
                                                                                                           BuckConfig buckConfig)
            ```

        []{#buildWithXcodeToolFinder(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.apple.toolchain.AppleSdk,java.lang.String,java.lang.String,com.facebook.buck.apple.toolchain.AppleSdkPaths,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.apple.toolchain.impl.XcodeToolFinder,com.facebook.buck.apple.toolchain.impl.AppleCxxPlatforms.XcodeBuildVersionCache)}

        -   #### buildWithXcodeToolFinder

            ``` methodSignature
            public static AppleCxxPlatform buildWithXcodeToolFinder​(ProjectFilesystem filesystem,
                                                                    AppleSdk targetSdk,
                                                                    String minVersion,
                                                                    String targetArchitecture,
                                                                    AppleSdkPaths sdkPaths,
                                                                    BuckConfig buckConfig,
                                                                    XcodeToolFinder xcodeToolFinder,
                                                                    AppleCxxPlatforms.XcodeBuildVersionCache xcodeBuildVersionCache)
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
