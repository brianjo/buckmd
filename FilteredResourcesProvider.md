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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface FilteredResourcesProvider {#interface-filteredresourcesprovider .title title="Interface FilteredResourcesProvider"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `IdentityResourcesProvider`, `ResourcesFilter`

    ------------------------------------------------------------------------

        public interface FilteredResourcesProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                   Description
          --------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------ -------------
          `Optional<SourcePath>`                                    `getOverrideSymbolsPath()`                                                                                                
          `default com.google.common.collect.ImmutableList<Path>`   `getRelativeResDirectories​(ProjectFilesystem filesystem,                          SourcePathResolverAdapter resolver)`    
          `com.google.common.collect.ImmutableList<SourcePath>`     `getResDirectories()`                                                                                                     
          `Optional<BuildRule>`                                     `getResourceFilterRule()`                                                                                                 
          `com.google.common.collect.ImmutableList<Path>`           `getStringFiles()`                                                                                                        
          `boolean`                                                 `hasResources()`                                                                                                          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResDirectories()}

        -   #### getResDirectories

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getResDirectories()
            ```

            [Returns:]{.returnLabel}
            :   The set of res/ directories that should be used to
                calculate the final R.java file.

        []{#getRelativeResDirectories(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getRelativeResDirectories

            ``` methodSignature
            default com.google.common.collect.ImmutableList<Path> getRelativeResDirectories​(ProjectFilesystem filesystem,
                                                                                            SourcePathResolverAdapter resolver)
            ```

        []{#getStringFiles()}

        -   #### getStringFiles

            ``` methodSignature
            com.google.common.collect.ImmutableList<Path> getStringFiles()
            ```

            [Returns:]{.returnLabel}
            :   The list of `strings.xml` files excluding whitelisted
                strings. Empty unless
                `ResourceCompressionMode.isStoreStringsAsAssets` is
                true.

        []{#getResourceFilterRule()}

        -   #### getResourceFilterRule

            ``` methodSignature
            Optional<BuildRule> getResourceFilterRule()
            ```

        []{#hasResources()}

        -   #### hasResources

            ``` methodSignature
            boolean hasResources()
            ```

        []{#getOverrideSymbolsPath()}

        -   #### getOverrideSymbolsPath

            ``` methodSignature
            Optional<SourcePath> getOverrideSymbolsPath()
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
