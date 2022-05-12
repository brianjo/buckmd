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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.manifest](package-summary.html)
:::

## Interface ManifestStoreResult {#interface-manifeststoreresult .title title="Interface ManifestStoreResult"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ManifestStoreResult

    ::: block
    Provides a results summary of a manifest-based cache store/update
    process.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                       Description
          ------------------- ------------------------------- -------------
          `static class `     `ManifestStoreResult.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                      Method                     Description
          ---------------------------------------------------------------------- -------------------------- -------------
          `static ManifestStoreResult.Builder`                                   `builder()`                 
          `default void`                                                         `check()`                   
          `boolean`                                                              `didCreateNewManifest()`    
          `Optional<String>`                                                     `getManifestLoadError()`    
          `ManifestStats`                                                        `getManifestStats()`        
          `Optional<com.google.common.util.concurrent.ListenableFuture<Unit>>`   `getStoreFuture()`          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            default void check()
            ```

        []{#didCreateNewManifest()}

        -   #### didCreateNewManifest

            ``` methodSignature
            boolean didCreateNewManifest()
            ```

            [Returns:]{.returnLabel}
            :   whether an existing manifest was updated, or a new one
                was stored.

        []{#getManifestStats()}

        -   #### getManifestStats

            ``` methodSignature
            ManifestStats getManifestStats()
            ```

            [Returns:]{.returnLabel}
            :   stats for the stored manifest.

        []{#getManifestLoadError()}

        -   #### getManifestLoadError

            ``` methodSignature
            Optional<String> getManifestLoadError()
            ```

            [Returns:]{.returnLabel}
            :   the error generated when trying to load an existing
                manifest.

        []{#getStoreFuture()}

        -   #### getStoreFuture

            ``` methodSignature
            Optional<com.google.common.util.concurrent.ListenableFuture<Unit>> getStoreFuture()
            ```

            [Returns:]{.returnLabel}
            :   a future wrapping the asynchronous cache upload.

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static ManifestStoreResult.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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
