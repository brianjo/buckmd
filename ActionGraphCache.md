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
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Class ActionGraphCache {#class-actiongraphcache .title title="Class ActionGraphCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.actiongraph.computation.ActionGraphCache

::: description
-   

    ------------------------------------------------------------------------

        public class ActionGraphCache
        extends Object

    ::: block
    Contains cached action graphs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                          Description
          ------------------------------------ -------------
          `ActionGraphCache​(int maxEntries)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                                                                                                                           Description
          ------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ActionGraphAndBuilder`   `getIfPresent​(TargetGraph targetGraph)`                                                                                                                                                                           
          `void`                    `invalidateCache()`                                                                                                                                                                                               
          `boolean`                 `isEmpty()`                                                                                                                                                                                                       
          `void`                    `populateActionGraphBuilderWithCachedRules​(BuckEventBus eventBus,                                          TargetGraph targetGraph,                                          ActionGraphBuilder graphBuilder)`    
          `void`                    `put​(TargetGraph targetGraph,    ActionGraphAndBuilder actionGraphAndBuilder)`                                                                                                                                    
          `long`                    `size()`                                                                                                                                                                                                          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(int)}

        -   #### ActionGraphCache

                public ActionGraphCache​(int maxEntries)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#invalidateCache()}

        -   #### invalidateCache

            ``` methodSignature
            public void invalidateCache()
            ```

        []{#getIfPresent(com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### getIfPresent

            ``` methodSignature
            @Nullable
            public ActionGraphAndBuilder getIfPresent​(TargetGraph targetGraph)
            ```

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#size()}

        -   #### size

            ``` methodSignature
            public long size()
            ```

        []{#put(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.actiongraph.ActionGraphAndBuilder)}

        -   #### put

            ``` methodSignature
            public void put​(TargetGraph targetGraph,
                            ActionGraphAndBuilder actionGraphAndBuilder)
            ```

        []{#populateActionGraphBuilderWithCachedRules(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### populateActionGraphBuilderWithCachedRules

            ``` methodSignature
            public void populateActionGraphBuilderWithCachedRules​(BuckEventBus eventBus,
                                                                  TargetGraph targetGraph,
                                                                  ActionGraphBuilder graphBuilder)
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
-   Nested \| 
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
