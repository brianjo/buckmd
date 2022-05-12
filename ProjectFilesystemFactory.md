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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem](package-summary.html)
:::

## Interface ProjectFilesystemFactory {#interface-projectfilesystemfactory .title title="Interface ProjectFilesystemFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultProjectFilesystemFactory`

    ------------------------------------------------------------------------

        public interface ProjectFilesystemFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                                                                                                                                                                                                                                                              Description
          --------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProjectFilesystem`   `createOrThrow​(CanonicalCellName cellName,              AbsPath path,              boolean buckOutIncludeTargetCofigHash)`                                                                                                                                                           
          `ProjectFilesystem`   `createProjectFilesystem​(CanonicalCellName cellName,                        AbsPath root,                        boolean buckOutIncludeTargetCofigHash)`                                                                                                                             
          `ProjectFilesystem`   `createProjectFilesystem​(CanonicalCellName cellName,                        AbsPath root,                        Config config,                        boolean buckOutIncludeTargetConfigHash)`                                                                                      
          `ProjectFilesystem`   `createProjectFilesystem​(CanonicalCellName cellName,                        AbsPath root,                        Config config,                        Optional<EmbeddedCellBuckOutInfo> embeddedCellBuckOutInfo,                        boolean buckOutIncludeTargetConfigHash)`    

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

        []{#createProjectFilesystem(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config,java.util.Optional,boolean)}

        -   #### createProjectFilesystem

            ``` methodSignature
            ProjectFilesystem createProjectFilesystem​(CanonicalCellName cellName,
                                                      AbsPath root,
                                                      Config config,
                                                      Optional<EmbeddedCellBuckOutInfo> embeddedCellBuckOutInfo,
                                                      boolean buckOutIncludeTargetConfigHash)
            ```

        []{#createProjectFilesystem(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config,boolean)}

        -   #### createProjectFilesystem

            ``` methodSignature
            ProjectFilesystem createProjectFilesystem​(CanonicalCellName cellName,
                                                      AbsPath root,
                                                      Config config,
                                                      boolean buckOutIncludeTargetConfigHash)
            ```

        []{#createProjectFilesystem(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,boolean)}

        -   #### createProjectFilesystem

            ``` methodSignature
            ProjectFilesystem createProjectFilesystem​(CanonicalCellName cellName,
                                                      AbsPath root,
                                                      boolean buckOutIncludeTargetCofigHash)
            ```

        []{#createOrThrow(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,boolean)}

        -   #### createOrThrow

            ``` methodSignature
            ProjectFilesystem createOrThrow​(CanonicalCellName cellName,
                                            AbsPath path,
                                            boolean buckOutIncludeTargetCofigHash)
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
