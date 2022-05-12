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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model.folders](package-summary.html)
:::

## Class ResourceFolder {#class-resourcefolder .title title="Class ResourceFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.model.folders.IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

    -   -   [com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder](InclusiveFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

        -   -   com.facebook.buck.features.project.intellij.model.folders.ResourceFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjFolder>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `JavaResourceFolder`, `JavaTestResourceFolder`

    ------------------------------------------------------------------------

        public abstract class ResourceFolder
        extends InclusiveFolder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field             Description
          ------------------- ----------------- -------------
          `protected Path`    `resourcesRoot`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                           Description
          ---------------------------------- -------------------------------- -------------
          `boolean`                          `canMergeWith​(IjFolder other)`    
          `boolean`                          `equals​(Object other)`            
          `Path`                             `getRelativeOutputPath()`         
          `abstract ResourceFolderFactory`   `getResourceFactory()`            
          `abstract IjResourceFolderType`    `getResourceFolderType()`         
          `Path`                             `getResourcesRoot()`              
          `int`                              `hashCode()`                      
          `boolean`                          `isResourceFolder()`              
          `IjFolder`                         `merge​(IjFolder otherFolder)`     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.model.folders.[InclusiveFolder](InclusiveFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `getIjName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.IjFolder}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.model.folders.[IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `combineInputs, compareTo, createCopyWith, getFactory, getInputs, getPath, getWantsPackagePrefix, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#resourcesRoot}

        -   #### resourcesRoot

                protected final Path resourcesRoot
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRelativeOutputPath()}

        -   #### getRelativeOutputPath

            ``` methodSignature
            public Path getRelativeOutputPath()
            ```

        []{#getResourcesRoot()}

        -   #### getResourcesRoot

            ``` methodSignature
            public Path getResourcesRoot()
            ```

        []{#isResourceFolder()}

        -   #### isResourceFolder

            ``` methodSignature
            public boolean isResourceFolder()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isResourceFolder` in class `IjFolder`

            [Returns:]{.returnLabel}
            :   true if it should be marked as a java-resource or
                java-test-resource folder, false otherwise.

        []{#merge(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### merge

            ``` methodSignature
            public IjFolder merge​(IjFolder otherFolder)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `merge` in class `IjFolder`

        []{#canMergeWith(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### canMergeWith

            ``` methodSignature
            public boolean canMergeWith​(IjFolder other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `canMergeWith` in class `IjFolder`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `IjFolder`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `IjFolder`

        []{#getResourceFolderType()}

        -   #### getResourceFolderType

            ``` methodSignature
            public abstract IjResourceFolderType getResourceFolderType()
            ```

        []{#getResourceFactory()}

        -   #### getResourceFactory

            ``` methodSignature
            public abstract ResourceFolderFactory getResourceFactory()
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
