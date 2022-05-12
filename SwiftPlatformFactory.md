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
[Package]{.packageLabelInType} [com.facebook.buck.swift.toolchain.impl](package-summary.html)
:::

## Class SwiftPlatformFactory {#class-swiftplatformfactory .title title="Class SwiftPlatformFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.toolchain.impl.SwiftPlatformFactory

::: description
-   

    ------------------------------------------------------------------------

        public class SwiftPlatformFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                                                                                              Description
          ------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static SwiftPlatform`    `build​(AppleSdk sdk,      AppleSdkPaths sdkPaths,      Tool swiftc,      Optional<Tool> swiftStdLibTool,      boolean shouldLinkSystemSwift,      SwiftTargetTriple swiftTarget)`    
          `static Optional<Path>`   `findSwiftCompatibilityRuntimePath​(Path toolchainPath,                                  String platformName)`                                                                        
          `static Optional<Path>`   `findSwiftRuntimePath​(Path toolchainPath,                     String platformName)`                                                                                                  

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

        []{#build(com.facebook.buck.apple.toolchain.AppleSdk,com.facebook.buck.apple.toolchain.AppleSdkPaths,com.facebook.buck.core.toolchain.tool.Tool,java.util.Optional,boolean,com.facebook.buck.swift.toolchain.SwiftTargetTriple)}

        -   #### build

            ``` methodSignature
            public static SwiftPlatform build​(AppleSdk sdk,
                                              AppleSdkPaths sdkPaths,
                                              Tool swiftc,
                                              Optional<Tool> swiftStdLibTool,
                                              boolean shouldLinkSystemSwift,
                                              SwiftTargetTriple swiftTarget)
            ```

        []{#findSwiftRuntimePath(java.nio.file.Path,java.lang.String)}

        -   #### findSwiftRuntimePath

            ``` methodSignature
            public static Optional<Path> findSwiftRuntimePath​(Path toolchainPath,
                                                              String platformName)
            ```

        []{#findSwiftCompatibilityRuntimePath(java.nio.file.Path,java.lang.String)}

        -   #### findSwiftCompatibilityRuntimePath

            ``` methodSignature
            public static Optional<Path> findSwiftCompatibilityRuntimePath​(Path toolchainPath,
                                                                           String platformName)
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
