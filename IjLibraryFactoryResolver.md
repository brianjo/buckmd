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

## Interface IjLibraryFactoryResolver {#interface-ijlibraryfactoryresolver .title title="Interface IjLibraryFactoryResolver"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface IjLibraryFactoryResolver
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getP                 | ::: block             |
        |                       | ath​(SourcePath path)` | Does it get an        |
        |                       |                       | absolute path? Does   |
        |                       |                       | it get a relative     |
        |                       |                       | path? Who knows!      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPa                |                       |
        | Optional<SourcePath>` | thIfJavaLibrary​(Targe |                       |
        |                       | tNode<?> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getPath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getPath

            ``` methodSignature
            Path getPath​(SourcePath path)
            ```

            ::: block
            Does it get an absolute path? Does it get a relative path?
            Who knows!
            :::

        []{#getPathIfJavaLibrary(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getPathIfJavaLibrary

            ``` methodSignature
            Optional<SourcePath> getPathIfJavaLibrary​(TargetNode<?> targetNode)
            ```

            [Parameters:]{.paramLabel}
            :   `targetNode` - node to look up.

            [Returns:]{.returnLabel}
            :   path to the output of target but only if that path
                points to a .jar.
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
