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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model.folders](package-summary.html)
:::

## Class SelfMergingOnlyFolder {#class-selfmergingonlyfolder .title title="Class SelfMergingOnlyFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.model.folders.IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

    -   -   [com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder](InclusiveFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

        -   -   com.facebook.buck.features.project.intellij.model.folders.SelfMergingOnlyFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjFolder>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AndroidResourceFolder`

    ------------------------------------------------------------------------

        public abstract class SelfMergingOnlyFolder
        extends InclusiveFolder

    ::: block
    Base class for folders which can only be merged with other instances
    holding equal data.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SelfMergingOnlyFolder​(Path path)`                                                                                                                                     
          `SelfMergingOnlyFolder​(Path path,                      boolean wantsPackagePrefix,                      com.google.common.collect.ImmutableSortedSet<Path> inputs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                           Description
          ------------------- -------------------------------- -------------
          `boolean`           `canMergeWith​(IjFolder other)`    
          `IjFolder`          `merge​(IjFolder otherFolder)`     

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

            `combineInputs, compareTo, createCopyWith, equals, getFactory, getInputs, getPath, getWantsPackagePrefix, hashCode, isResourceFolder, toString`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,boolean,com.google.common.collect.ImmutableSortedSet)}

        -   #### SelfMergingOnlyFolder

                public SelfMergingOnlyFolder​(Path path,
                                             boolean wantsPackagePrefix,
                                             com.google.common.collect.ImmutableSortedSet<Path> inputs)

        []{#<init>(java.nio.file.Path)}

        -   #### SelfMergingOnlyFolder

                public SelfMergingOnlyFolder​(Path path)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#canMergeWith(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### canMergeWith

            ``` methodSignature
            public boolean canMergeWith​(IjFolder other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `canMergeWith` in class `IjFolder`

        []{#merge(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### merge

            ``` methodSignature
            public IjFolder merge​(IjFolder otherFolder)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `merge` in class `IjFolder`
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
