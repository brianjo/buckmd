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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.context](package-summary.html)
:::

## Class BuildContext {#class-buildcontext .title title="Class BuildContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.context.BuildContext

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildContext
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `BuildContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                                                                                                                            Description
          -------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract Path`                        `getBuildCellRootPath()`                                                                                                                                                           
          `abstract BuckEventBus`                `getEventBus()`                                                                                                                                                                    
          `abstract JavaPackageFinder`           `getJavaPackageFinder()`                                                                                                                                                           
          `abstract boolean`                     `getShouldDeleteTemporaries()`                                                                                                                                                     
          `abstract SourcePathResolverAdapter`   `getSourcePathResolver()`                                                                                                                                                          
          `static BuildContext`                  `of​(SourcePathResolverAdapter sourcePathResolver,   Path buildCellRootPath,   JavaPackageFinder javaPackageFinder,   BuckEventBus eventBus,   boolean shouldDeleteTemporaries)`    
          `BuildContext`                         `withBuildCellRootPath​(Path buildCellRootPath)`                                                                                                                                    
          `BuildContext`                         `withEventBus​(BuckEventBus eventBus)`                                                                                                                                              
          `BuildContext`                         `withJavaPackageFinder​(JavaPackageFinder javaPackageFinder)`                                                                                                                       
          `BuildContext`                         `withSourcePathResolver​(SourcePathResolverAdapter sourcePathResolver)`                                                                                                             

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

        -   #### BuildContext

                public BuildContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePathResolver()}

        -   #### getSourcePathResolver

            ``` methodSignature
            public abstract SourcePathResolverAdapter getSourcePathResolver()
            ```

        []{#getBuildCellRootPath()}

        -   #### getBuildCellRootPath

            ``` methodSignature
            public abstract Path getBuildCellRootPath()
            ```

            [Returns:]{.returnLabel}
            :   the absolute path of the cell in which the build was
                invoked.

        []{#getJavaPackageFinder()}

        -   #### getJavaPackageFinder

            ``` methodSignature
            public abstract JavaPackageFinder getJavaPackageFinder()
            ```

        []{#getEventBus()}

        -   #### getEventBus

            ``` methodSignature
            public abstract BuckEventBus getEventBus()
            ```

        []{#getShouldDeleteTemporaries()}

        -   #### getShouldDeleteTemporaries

            ``` methodSignature
            public abstract boolean getShouldDeleteTemporaries()
            ```

        []{#of(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,com.facebook.buck.jvm.core.JavaPackageFinder,com.facebook.buck.event.BuckEventBus,boolean)}

        -   #### of

            ``` methodSignature
            public static BuildContext of​(SourcePathResolverAdapter sourcePathResolver,
                                          Path buildCellRootPath,
                                          JavaPackageFinder javaPackageFinder,
                                          BuckEventBus eventBus,
                                          boolean shouldDeleteTemporaries)
            ```

        []{#withBuildCellRootPath(java.nio.file.Path)}

        -   #### withBuildCellRootPath

            ``` methodSignature
            public BuildContext withBuildCellRootPath​(Path buildCellRootPath)
            ```

        []{#withEventBus(com.facebook.buck.event.BuckEventBus)}

        -   #### withEventBus

            ``` methodSignature
            public BuildContext withEventBus​(BuckEventBus eventBus)
            ```

        []{#withJavaPackageFinder(com.facebook.buck.jvm.core.JavaPackageFinder)}

        -   #### withJavaPackageFinder

            ``` methodSignature
            public BuildContext withJavaPackageFinder​(JavaPackageFinder javaPackageFinder)
            ```

        []{#withSourcePathResolver(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### withSourcePathResolver

            ``` methodSignature
            public BuildContext withSourcePathResolver​(SourcePathResolverAdapter sourcePathResolver)
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
