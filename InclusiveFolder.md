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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model.folders](package-summary.html)
:::

## Class InclusiveFolder {#class-inclusivefolder .title title="Class InclusiveFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.model.folders.IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

    -   -   com.facebook.buck.features.project.intellij.model.folders.InclusiveFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjFolder>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ResourceFolder`, `SelfMergingOnlyFolder`, `SourceFolder`,
        `TestFolder`

    ------------------------------------------------------------------------

        public abstract class InclusiveFolder
        extends IjFolder

    ::: block
    A path which contains a set of sources we wish to present to
    IntelliJ.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method          Description
          ------------------- --------------- -------------
          `String`            `getIjName()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.folders.IjFolder}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.model.folders.[IjFolder](IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")

            `canMergeWith, combineInputs, compareTo, createCopyWith, equals, getFactory, getInputs, getPath, getWantsPackagePrefix, hashCode, isResourceFolder, merge, toString`

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
    -   []{#method.detail}

        ### Method Detail

        []{#getIjName()}

        -   #### getIjName

            ``` methodSignature
            public String getIjName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIjName` in class `IjFolder`

            [Returns:]{.returnLabel}
            :   name IntelliJ would use to refer to this type of folder.
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
