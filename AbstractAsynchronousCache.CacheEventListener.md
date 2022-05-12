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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Interface AbstractAsynchronousCache.CacheEventListener {#interface-abstractasynchronouscache.cacheeventlistener .title title="Interface AbstractAsynchronousCache.CacheEventListener"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [AbstractAsynchronousCache](AbstractAsynchronousCache.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static interface AbstractAsynchronousCache.CacheEventListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                                                                Description
          --------------------- ------------------------------------------------------------------------ -------------
          `static interface `   `AbstractAsynchronousCache.CacheEventListener.FetchRequestEvents`         
          `static interface `   `AbstractAsynchronousCache.CacheEventListener.MultiFetchRequestEvents`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                        Method                                                                                                                                                      Description
          ------------------------------------------------------------------------ ----------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                                                                   `fetchScheduled​(RuleKey ruleKey)`                                                                                                                            
          `AbstractAsynchronousCache.CacheEventListener.FetchRequestEvents`        `fetchStarted​(BuildTarget target,             RuleKey ruleKey)`                                                                                              
          `AbstractAsynchronousCache.CacheEventListener.MultiFetchRequestEvents`   `multiFetchStarted​(com.google.common.collect.ImmutableList<BuildTarget> targets,                  com.google.common.collect.ImmutableList<RuleKey> keys)`    
          `AbstractAsynchronousCache.StoreEvents`                                  `storeScheduled​(ArtifactInfo info,               long artifactSizeBytes)`                                                                                    

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

        []{#storeScheduled(com.facebook.buck.artifact_cache.ArtifactInfo,long)}

        -   #### storeScheduled

            ``` methodSignature
            AbstractAsynchronousCache.StoreEvents storeScheduled​(ArtifactInfo info,
                                                                 long artifactSizeBytes)
            ```

        []{#fetchScheduled(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### fetchScheduled

            ``` methodSignature
            void fetchScheduled​(RuleKey ruleKey)
            ```

        []{#fetchStarted(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey)}

        -   #### fetchStarted

            ``` methodSignature
            AbstractAsynchronousCache.CacheEventListener.FetchRequestEvents fetchStarted​(BuildTarget target,
                                                                                         RuleKey ruleKey)
            ```

        []{#multiFetchStarted(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### multiFetchStarted

            ``` methodSignature
            AbstractAsynchronousCache.CacheEventListener.MultiFetchRequestEvents multiFetchStarted​(com.google.common.collect.ImmutableList<BuildTarget> targets,
                                                                                                   com.google.common.collect.ImmutableList<RuleKey> keys)
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
