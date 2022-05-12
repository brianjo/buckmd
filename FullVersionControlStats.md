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
[Package]{.packageLabelInType} [com.facebook.buck.util.versioncontrol](package-summary.html)
:::

## Interface FullVersionControlStats {#interface-fullversioncontrolstats .title title="Interface FullVersionControlStats"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `CommonFastVersionControlStats`, `CommonSlowVersionControlStats`

    ------------------------------------------------------------------------

        public interface FullVersionControlStats
        extends CommonSlowVersionControlStats
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                           Description
          ------------------- ----------------------------------- -------------
          `static class `     `FullVersionControlStats.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method        Description
          ------------------------------------------------- ------------- -------------
          `static FullVersionControlStats.Builder`          `builder()`    
          `Optional<VersionControlSupplier<InputStream>>`   `getDiff()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.versioncontrol.CommonFastVersionControlStats}

            ### Methods inherited from interface com.facebook.buck.util.versioncontrol.[CommonFastVersionControlStats](CommonFastVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol")

            `getBaseBookmarks, getBranchedFromMasterRevisionId, getBranchedFromMasterTS, getCurrentRevisionId`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.util.versioncontrol.CommonSlowVersionControlStats}

            ### Methods inherited from interface com.facebook.buck.util.versioncontrol.[CommonSlowVersionControlStats](CommonSlowVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol")

            `getPathsChangedInWorkingDirectory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDiff()}

        -   #### getDiff

            ``` methodSignature
            Optional<VersionControlSupplier<InputStream>> getDiff()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static FullVersionControlStats.Builder builder()
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
