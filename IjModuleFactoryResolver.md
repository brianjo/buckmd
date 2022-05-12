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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Interface IjModuleFactoryResolver {#interface-ijmodulefactoryresolver .title title="Interface IjModuleFactoryResolver"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface IjModuleFactoryResolver

    ::: block
    Provides the
    [`IjModuleFactory`](IjModuleFactory.html "interface in com.facebook.buck.features.project.intellij.model")
    with
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
    to various elements of the project.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                      Description
          ------------------- ------------------------------------------------------------------------------------------- -------------
          `Path`              `getAndroidManifestPath​(TargetNode<AndroidBinaryDescriptionArg> targetNode)`                 
          `Optional<Path>`    `getAndroidResourcePath​(TargetNode<AndroidResourceDescriptionArg> targetNode)`               
          `Optional<Path>`    `getAnnotationOutputPath​(TargetNode<? extends JvmLibraryArg> targetNode)`                    
          `Optional<Path>`    `getAssetsPath​(TargetNode<AndroidResourceDescriptionArg> targetNode)`                        
          `Optional<Path>`    `getCompilerOutputPath​(TargetNode<? extends JvmLibraryArg> targetNode)`                      
          `Optional<Path>`    `getDummyRDotJavaPath​(TargetNode<?> targetNode)`                                             
          `Optional<Path>`    `getKaptAnnotationOutputPath​(TargetNode<? extends JvmLibraryArg> targetNode)`                
          `Optional<Path>`    `getLibraryAndroidManifestPath​(TargetNode<AndroidLibraryDescription.CoreArg> targetNode)`    
          `Optional<Path>`    `getProguardConfigPath​(TargetNode<AndroidBinaryDescriptionArg> targetNode)`                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDummyRDotJavaPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getDummyRDotJavaPath

            ``` methodSignature
            Optional<Path> getDummyRDotJavaPath​(TargetNode<?> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node to generate the path to

            [Returns:]{.returnLabel}
            :   the project-relative path to a directory structure under
                which the R.class file can be found (the structure will
                be the same as the package path of the R class). A path
                should be returned only if the given TargetNode requires
                the R.class to compile.

        []{#getAndroidManifestPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getAndroidManifestPath

            ``` methodSignature
            Path getAndroidManifestPath​(TargetNode<AndroidBinaryDescriptionArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node describing the Android binary to get
                the manifest of.

            [Returns:]{.returnLabel}
            :   path on disk to the AndroidManifest.

        []{#getLibraryAndroidManifestPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getLibraryAndroidManifestPath

            ``` methodSignature
            Optional<Path> getLibraryAndroidManifestPath​(TargetNode<AndroidLibraryDescription.CoreArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node describing the Android library to
                get the manifest of.

            [Returns:]{.returnLabel}
            :   path on disk to the AndroidManifest.

        []{#getProguardConfigPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getProguardConfigPath

            ``` methodSignature
            Optional<Path> getProguardConfigPath​(TargetNode<AndroidBinaryDescriptionArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node describing the Android binary to get
                the Proguard config of.

            [Returns:]{.returnLabel}
            :   path on disk to the proguard config.

        []{#getAndroidResourcePath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getAndroidResourcePath

            ``` methodSignature
            Optional<Path> getAndroidResourcePath​(TargetNode<AndroidResourceDescriptionArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node describing the Android resources to
                get the path of.

            [Returns:]{.returnLabel}
            :   path on disk to the resources folder.

        []{#getAssetsPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getAssetsPath

            ``` methodSignature
            Optional<Path> getAssetsPath​(TargetNode<AndroidResourceDescriptionArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node describing the Android assets to get
                the path of.

            [Returns:]{.returnLabel}
            :   path on disk to the assets folder.

        []{#getAnnotationOutputPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getAnnotationOutputPath

            ``` methodSignature
            Optional<Path> getAnnotationOutputPath​(TargetNode<? extends JvmLibraryArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node which may use annotation processors.

            [Returns:]{.returnLabel}
            :   path to the annotation processor output if any
                annotation proceessors are configured for the given
                node.

        []{#getKaptAnnotationOutputPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getKaptAnnotationOutputPath

            ``` methodSignature
            Optional<Path> getKaptAnnotationOutputPath​(TargetNode<? extends JvmLibraryArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node which may use annotation processors.

            [Returns:]{.returnLabel}
            :   path to the kapt output if any annotation proceessors
                are configured for the given node.

        []{#getCompilerOutputPath(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getCompilerOutputPath

            ``` methodSignature
            Optional<Path> getCompilerOutputPath​(TargetNode<? extends JvmLibraryArg> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node which may specify it\'s own compiler
                output path.

            [Returns:]{.returnLabel}
            :   path to the classes that make up the compiler output.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
