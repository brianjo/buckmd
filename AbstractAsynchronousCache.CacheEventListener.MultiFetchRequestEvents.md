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
-   [Field](#field.summary) \| 
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

## Interface AbstractAsynchronousCache.CacheEventListener.MultiFetchRequestEvents {#interface-abstractasynchronouscache.cacheeventlistener.multifetchrequestevents .title title="Interface AbstractAsynchronousCache.CacheEventListener.MultiFetchRequestEvents"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Scope`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [AbstractAsynchronousCache.CacheEventListener](AbstractAsynchronousCache.CacheEventListener.html "interface in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static interface AbstractAsynchronousCache.CacheEventListener.MultiFetchRequestEvents
        extends Scope
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.util.Scope}

            ### Fields inherited from interface com.facebook.buck.util.[Scope](../util/Scope.html "interface in com.facebook.buck.util")

            `NOOP`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                Description
          ------------------- --------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `failed​(int keyIndex,       IOException e,       String msg,       CacheResult result)`                                
          `void`              `finished​(int keyIndex,         com.facebook.buck.artifact_cache.AbstractAsynchronousCache.FetchResult thisResult)`    
          `void`              `skipped​(int keyIndex)`                                                                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.Scope}

            ### Methods inherited from interface com.facebook.buck.util.[Scope](../util/Scope.html "interface in com.facebook.buck.util")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#skipped(int)}

        -   #### skipped

            ``` methodSignature
            void skipped​(int keyIndex)
            ```

        []{#finished(int,com.facebook.buck.artifact_cache.AbstractAsynchronousCache.FetchResult)}

        -   #### finished

            ``` methodSignature
            void finished​(int keyIndex,
                          com.facebook.buck.artifact_cache.AbstractAsynchronousCache.FetchResult thisResult)
            ```

        []{#failed(int,java.io.IOException,java.lang.String,com.facebook.buck.artifact_cache.CacheResult)}

        -   #### failed

            ``` methodSignature
            void failed​(int keyIndex,
                        IOException e,
                        String msg,
                        CacheResult result)
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
-   [Field](#field.summary) \| 
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
