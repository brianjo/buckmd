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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model.folders](package-summary.html)
:::

## Class JavaTestResourceFolder {#class-javatestresourcefolder .title title="Class JavaTestResourceFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.model.folders.IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

    -   -   [com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder](InclusiveFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

        -   -   [com.facebook.buck.features.project.intellij.model.folders.ResourceFolder](ResourceFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            -   -   com.facebook.buck.features.project.intellij.model.folders.JavaTestResourceFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjFolder>`

    ------------------------------------------------------------------------

        public class JavaTestResourceFolder
        extends ResourceFolder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                Field       Description
          -------------------------------- ----------- -------------
          `static ResourceFolderFactory`   `FACTORY`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.ResourceFolder}

            ### Fields inherited from class com.facebook.buck.features.project.intellij.model.folders.[ResourceFolder](ResourceFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `resourcesRoot`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                      Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaTestResourceFolder​(Path path,                       Path resourcesRoot,                       com.google.common.collect.ImmutableSortedSet<Path> inputs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                      Description
          ----------------------------- --------------------------- -------------
          `protected IJFolderFactory`   `getFactory()`               
          `ResourceFolderFactory`       `getResourceFactory()`       
          `IjResourceFolderType`        `getResourceFolderType()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.ResourceFolder}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.model.folders.[ResourceFolder](ResourceFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `canMergeWith, equals, getRelativeOutputPath, getResourcesRoot, hashCode, isResourceFolder, merge`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.model.folders.[InclusiveFolder](InclusiveFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `getIjName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.IjFolder}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.model.folders.[IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `combineInputs, compareTo, createCopyWith, getInputs, getPath, getWantsPackagePrefix, toString`

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

        []{#FACTORY}

        -   #### FACTORY

                public static final ResourceFolderFactory FACTORY
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableSortedSet)}

        -   #### JavaTestResourceFolder

                public JavaTestResourceFolder​(Path path,
                                              @Nullable
                                              Path resourcesRoot,
                                              com.google.common.collect.ImmutableSortedSet<Path> inputs)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResourceFolderType()}

        -   #### getResourceFolderType

            ``` methodSignature
            public IjResourceFolderType getResourceFolderType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourceFolderType` in class `ResourceFolder`

        []{#getFactory()}

        -   #### getFactory

            ``` methodSignature
            protected IJFolderFactory getFactory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFactory` in class `IjFolder`

            [Returns:]{.returnLabel}
            :   a IJFolderFactory to create new instances of the folder
                class.

        []{#getResourceFactory()}

        -   #### getResourceFactory

            ``` methodSignature
            public ResourceFolderFactory getResourceFactory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourceFactory` in class `ResourceFolder`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
