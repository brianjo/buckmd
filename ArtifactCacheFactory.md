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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Interface ArtifactCacheFactory {#interface-artifactcachefactory .title title="Interface ArtifactCacheFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ArtifactCaches`, `NoopArtifactCache.NoopArtifactCacheFactory`,
        `SingletonArtifactCacheFactory`

    ------------------------------------------------------------------------

        public interface ArtifactCacheFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                              Description
          ------------------------ ----------------------------------- -------------
          `ArtifactCacheFactory`   `cloneWith​(BuckConfig newConfig)`    
          `ArtifactCache`          `localOnlyInstance()`                
          `ArtifactCache`          `newInstance()`                      
          `ArtifactCache`          `remoteOnlyInstance()`               

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

        []{#newInstance()}

        -   #### newInstance

            ``` methodSignature
            ArtifactCache newInstance()
            ```

        []{#remoteOnlyInstance()}

        -   #### remoteOnlyInstance

            ``` methodSignature
            ArtifactCache remoteOnlyInstance()
            ```

        []{#localOnlyInstance()}

        -   #### localOnlyInstance

            ``` methodSignature
            ArtifactCache localOnlyInstance()
            ```

        []{#cloneWith(com.facebook.buck.core.config.BuckConfig)}

        -   #### cloneWith

            ``` methodSignature
            ArtifactCacheFactory cloneWith​(BuckConfig newConfig)
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