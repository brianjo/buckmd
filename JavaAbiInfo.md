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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Interface JavaAbiInfo {#interface-javaabiinfo .title title="Interface JavaAbiInfo"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultJavaAbiInfo`, `EmptyJavaAbiInfo`

    ------------------------------------------------------------------------

        public interface JavaAbiInfo

    ::: block
    Provides information about a java abi.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                           Description
          ------------------------------------------------------------ ------------------------------------------------ -------------
          `BuildTarget`                                                `getBuildTarget()`                                
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`   `getJarContents()`                                
          `void`                                                       `invalidate()`                                    
          `boolean`                                                    `jarContains​(String path)`                        
          `void`                                                       `load​(SourcePathResolverAdapter pathResolver)`    

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

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

        []{#getJarContents()}

        -   #### getJarContents

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<SourcePath> getJarContents()
            ```

        []{#jarContains(java.lang.String)}

        -   #### jarContains

            ``` methodSignature
            boolean jarContains​(String path)
            ```

        []{#load(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### load

            ``` methodSignature
            void load​(SourcePathResolverAdapter pathResolver)
               throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            void invalidate()
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
