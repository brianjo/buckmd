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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener.stats.cache](package-summary.html)
:::

## Class CacheRateStatsKeeper {#class-cacheratestatskeeper .title title="Class CacheRateStatsKeeper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.stats.cache.CacheRateStatsKeeper

::: description
-   

    ------------------------------------------------------------------------

        public class CacheRateStatsKeeper
        extends Object

    ::: block
    Measure CACHE HIT % based on total cache misses and the theoretical
    total number of build rules. REASON: If we only look at cache_misses
    and processed rules we are strongly biasing the result toward
    misses. Basically misses weight more than hits. One MISS will
    traverse all its dependency subtree potentially generating misses
    for all internal Nodes; worst case generating N cache_misses. One
    HIT will prevent any further traversal of dependency sub-tree nodes
    so it will only count as one cache_hit even though it saved us from
    fetching N nodes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                              Description
          ------------------- -------------------------------------------------- -------------
          `static class `     `CacheRateStatsKeeper.CacheRateStatsUpdateEvent`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `CacheRateStatsKeeper()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                     Description
          --------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`                                                    `buildRuleFinished​(BuildRuleEvent.Finished finished)`                                                                                       
          `static CacheRateStatsKeeper.CacheRateStatsUpdateEvent`   `getAggregatedCacheRateStats​(com.google.common.collect.ImmutableCollection<CacheRateStatsKeeper.CacheRateStatsUpdateEvent> statsEvents)`    
          `AtomicInteger`                                           `getRuleCount()`                                                                                                                            
          `CacheRateStatsKeeper.CacheRateStatsUpdateEvent`          `getStats()`                                                                                                                                
          `void`                                                    `ruleCountCalculated​(BuildEvent.RuleCountCalculated calculated)`                                                                            
          `void`                                                    `ruleCountUpdated​(BuildEvent.UnskippedRuleCountUpdated updated)`                                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CacheRateStatsKeeper

                public CacheRateStatsKeeper()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildRuleFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### buildRuleFinished

            ``` methodSignature
            public void buildRuleFinished​(BuildRuleEvent.Finished finished)
            ```

        []{#ruleCountCalculated(com.facebook.buck.core.build.event.BuildEvent.RuleCountCalculated)}

        -   #### ruleCountCalculated

            ``` methodSignature
            public void ruleCountCalculated​(BuildEvent.RuleCountCalculated calculated)
            ```

        []{#ruleCountUpdated(com.facebook.buck.core.build.event.BuildEvent.UnskippedRuleCountUpdated)}

        -   #### ruleCountUpdated

            ``` methodSignature
            public void ruleCountUpdated​(BuildEvent.UnskippedRuleCountUpdated updated)
            ```

        []{#getAggregatedCacheRateStats(com.google.common.collect.ImmutableCollection)}

        -   #### getAggregatedCacheRateStats

            ``` methodSignature
            public static CacheRateStatsKeeper.CacheRateStatsUpdateEvent getAggregatedCacheRateStats​(com.google.common.collect.ImmutableCollection<CacheRateStatsKeeper.CacheRateStatsUpdateEvent> statsEvents)
            ```

        []{#getStats()}

        -   #### getStats

            ``` methodSignature
            public CacheRateStatsKeeper.CacheRateStatsUpdateEvent getStats()
            ```

        []{#getRuleCount()}

        -   #### getRuleCount

            ``` methodSignature
            public AtomicInteger getRuleCount()
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
