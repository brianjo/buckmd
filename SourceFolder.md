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

## Class SourceFolder {#class-sourcefolder .title title="Class SourceFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.model.folders.IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

    -   -   [com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder](InclusiveFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

        -   -   com.facebook.buck.features.project.intellij.model.folders.SourceFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjFolder>`

    ------------------------------------------------------------------------

        public class SourceFolder
        extends InclusiveFolder

    ::: block
    A path which contains a set of sources we wish to present to
    IntelliJ.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type          Field       Description
          -------------------------- ----------- -------------
          `static IJFolderFactory`   `FACTORY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SourceFolder​(Path path)`                                                                                                                   
          `SourceFolder​(Path path,             boolean wantsPackagePrefix)`                                                                           
          `SourceFolder​(Path path,             boolean wantsPackagePrefix,             com.google.common.collect.ImmutableSortedSet<Path> inputs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method           Description
          ------------------- ---------------- -------------
          `IJFolderFactory`   `getFactory()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

            `canMergeWith, combineInputs, compareTo, createCopyWith, equals, getInputs, getPath, getWantsPackagePrefix, hashCode, isResourceFolder, merge, toString`

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

                public static final IJFolderFactory FACTORY
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,boolean,com.google.common.collect.ImmutableSortedSet)}

        -   #### SourceFolder

                public SourceFolder​(Path path,
                                    boolean wantsPackagePrefix,
                                    com.google.common.collect.ImmutableSortedSet<Path> inputs)

        []{#<init>(java.nio.file.Path,boolean)}

        -   #### SourceFolder

                public SourceFolder​(Path path,
                                    boolean wantsPackagePrefix)

        []{#<init>(java.nio.file.Path)}

        -   #### SourceFolder

                public SourceFolder​(Path path)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFactory()}

        -   #### getFactory

            ``` methodSignature
            public IJFolderFactory getFactory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFactory` in class `IjFolder`

            [Returns:]{.returnLabel}
            :   a IJFolderFactory to create new instances of the folder
                class.
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
