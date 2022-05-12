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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Interface FileHashCache.FileHashCacheVerificationResult {#interface-filehashcache.filehashcacheverificationresult .title title="Interface FileHashCache.FileHashCacheVerificationResult"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [FileHashCache](FileHashCache.html "interface in com.facebook.buck.util.cache")

    ------------------------------------------------------------------------

        public static interface FileHashCache.FileHashCacheVerificationResult
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                        Method                                                                                                                Description
          -------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------- -------------
          `int`                                                    `getCachesExamined()`                                                                                                  
          `int`                                                    `getFilesExamined()`                                                                                                   
          `com.google.common.collect.ImmutableList<String>`        `getVerificationErrors()`                                                                                              
          `static FileHashCache.FileHashCacheVerificationResult`   `of​(int cachesExamined,   int filesExamined)`                                                                          
          `static FileHashCache.FileHashCacheVerificationResult`   `of​(int cachesExamined,   int filesExamined,   com.google.common.collect.ImmutableList<String> verificationErrors)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCachesExamined()}

        -   #### getCachesExamined

            ``` methodSignature
            int getCachesExamined()
            ```

        []{#getFilesExamined()}

        -   #### getFilesExamined

            ``` methodSignature
            int getFilesExamined()
            ```

        []{#getVerificationErrors()}

        -   #### getVerificationErrors

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getVerificationErrors()
            ```

        []{#of(int,int)}

        -   #### of

            ``` methodSignature
            static FileHashCache.FileHashCacheVerificationResult of​(int cachesExamined,
                                                                    int filesExamined)
            ```

        []{#of(int,int,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            static FileHashCache.FileHashCacheVerificationResult of​(int cachesExamined,
                                                                    int filesExamined,
                                                                    com.google.common.collect.ImmutableList<String> verificationErrors)
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