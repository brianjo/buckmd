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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.cache.manager](package-summary.html)
:::

## Interface ManifestRuleKeyService {#interface-manifestrulekeyservice .title title="Interface ManifestRuleKeyService"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ManifestRuleKeyService

    ::: block
    Service in charge of persisting (fetch/store) the manifest for
    ManifestRuleKeys.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `c                    | `fetchManifest​(       | ::: block             |
        | om.google.common.util | RuleKey manifestKey,  | Reads the manifest    |
        | .concurrent.Listenabl |              LazyPath | used the              |
        | eFuture<CacheResult>` |  downloadedManifest)` | ManifestRuleKey from  |
        |                       |                       | some persistent       |
        |                       |                       | storage.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `store                | ::: block             |
        | on.util.concurrent.Li | Manifest​(RuleKey mani | Writes the manifest   |
        | stenableFuture<Unit>` | festKey,              | used the              |
        |                       |  Path manifestToUploa | ManifestRuleKey into  |
        |                       | d,              long  | some persistent       |
        |                       | artifactBuildTimeMs)` | storage.              |
        |                       |                       | :::                   |
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

        []{#storeManifest(com.facebook.buck.core.rulekey.RuleKey,java.nio.file.Path,long)}

        -   #### storeManifest

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> storeManifest​(RuleKey manifestKey,
                                                                                   Path manifestToUpload,
                                                                                   long artifactBuildTimeMs)
            ```

            ::: block
            Writes the manifest used the ManifestRuleKey into some
            persistent storage.
            :::

        []{#fetchManifest(com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetchManifest

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<CacheResult> fetchManifest​(RuleKey manifestKey,
                                                                                          LazyPath downloadedManifest)
            ```

            ::: block
            Reads the manifest used the ManifestRuleKey from some
            persistent storage.
            :::
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
