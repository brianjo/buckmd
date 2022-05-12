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
[Package]{.packageLabelInType} [com.facebook.buck.swift.toolchain](package-summary.html)
:::

## Interface SwiftPlatform {#interface-swiftplatform .title title="Interface SwiftPlatform"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface SwiftPlatform

    ::: block
    Interface describing a Swift toolchain and platform to build for.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                 Description
          ------------------- ------------------------- -------------
          `static class `     `SwiftPlatform.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                Description
          ------------------------------------------------- ------------------------------------- -------------
          `static SwiftPlatform.Builder`                    `builder()`                            
          `Tool`                                            `getSwiftc()`                          
          `com.google.common.collect.ImmutableSet<Path>`    `getSwiftRuntimePathsForBundling()`    
          `com.google.common.collect.ImmutableSet<Path>`    `getSwiftRuntimePathsForLinking()`     
          `com.google.common.collect.ImmutableList<Path>`   `getSwiftSharedLibraryRunPaths()`      
          `com.google.common.collect.ImmutableSet<Path>`    `getSwiftStaticRuntimePaths()`         
          `Optional<Tool>`                                  `getSwiftStdlibTool()`                 
          `SwiftTargetTriple`                               `getSwiftTarget()`                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSwiftc()}

        -   #### getSwiftc

            ``` methodSignature
            Tool getSwiftc()
            ```

        []{#getSwiftStdlibTool()}

        -   #### getSwiftStdlibTool

            ``` methodSignature
            Optional<Tool> getSwiftStdlibTool()
            ```

        []{#getSwiftRuntimePathsForBundling()}

        -   #### getSwiftRuntimePathsForBundling

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Path> getSwiftRuntimePathsForBundling()
            ```

            [Returns:]{.returnLabel}
            :   A set of directories which contain the Swift runtime as
                dynamic libraries. On macOS, the directory will contain
                libs like libswiftCore.dylib and others. The libs will
                be passed to swift-stdlib-tool for inclusion in the app
                bundle.

        []{#getSwiftRuntimePathsForLinking()}

        -   #### getSwiftRuntimePathsForLinking

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Path> getSwiftRuntimePathsForLinking()
            ```

            [Returns:]{.returnLabel}
            :   A set of directories which contain the Swift runtime as
                dynamic libraries. On macOS, the directory will contain
                the .tbd libs like libSwiftCore.tbd and others. The libs
                will be passed during the link step.

        []{#getSwiftStaticRuntimePaths()}

        -   #### getSwiftStaticRuntimePaths

            ``` methodSignature
            com.google.common.collect.ImmutableSet<Path> getSwiftStaticRuntimePaths()
            ```

            [Returns:]{.returnLabel}
            :   A set of directories which contain the Swift runtime as
                static libraries. On macOS, the directory will contain
                libs like libswiftCore.a and others.

        []{#getSwiftSharedLibraryRunPaths()}

        -   #### getSwiftSharedLibraryRunPaths

            ``` methodSignature
            com.google.common.collect.ImmutableList<Path> getSwiftSharedLibraryRunPaths()
            ```

            [Returns:]{.returnLabel}
            :   A set of search paths used by the dynamic linker loader
                to find of linked shared libraries. Each of the paths is
                usually referred as an \"rpath\". For example, on iOS,
                \"@executable_path/Frameworks\" is a common rpath.

        []{#getSwiftTarget()}

        -   #### getSwiftTarget

            ``` methodSignature
            SwiftTargetTriple getSwiftTarget()
            ```

            [Returns:]{.returnLabel}
            :   Structure that represents the architecture target the
                swift module is built for e.g. x86_64-apple-ios9.0

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static SwiftPlatform.Builder builder()
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
