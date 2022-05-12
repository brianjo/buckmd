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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Interface GroupedSource.Visitor {#interface-groupedsource.visitor .title title="Interface GroupedSource.Visitor"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [GroupedSource](GroupedSource.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        public static interface GroupedSource.Visitor
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                              Description
          ------------------- --------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `visitIgnoredSource​(SourcePath source)`                                                                                                              
          `void`              `visitPrivateHeader​(SourcePath privateHeader)`                                                                                                       
          `void`              `visitPublicHeader​(SourcePath publicHeader)`                                                                                                         
          `void`              `visitSourceGroup​(String sourceGroupName,                 Path sourceGroupPathRelativeToTarget,                 List<GroupedSource> sourceGroup)`    
          `void`              `visitSourceWithFlags​(SourceWithFlags sourceWithFlags)`                                                                                              

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

        []{#visitSourceWithFlags(com.facebook.buck.core.sourcepath.SourceWithFlags)}

        -   #### visitSourceWithFlags

            ``` methodSignature
            void visitSourceWithFlags​(SourceWithFlags sourceWithFlags)
            ```

        []{#visitIgnoredSource(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### visitIgnoredSource

            ``` methodSignature
            void visitIgnoredSource​(SourcePath source)
            ```

        []{#visitPublicHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### visitPublicHeader

            ``` methodSignature
            void visitPublicHeader​(SourcePath publicHeader)
            ```

        []{#visitPrivateHeader(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### visitPrivateHeader

            ``` methodSignature
            void visitPrivateHeader​(SourcePath privateHeader)
            ```

        []{#visitSourceGroup(java.lang.String,java.nio.file.Path,java.util.List)}

        -   #### visitSourceGroup

            ``` methodSignature
            void visitSourceGroup​(String sourceGroupName,
                                  Path sourceGroupPathRelativeToTarget,
                                  List<GroupedSource> sourceGroup)
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
