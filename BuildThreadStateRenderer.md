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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class BuildThreadStateRenderer {#class-buildthreadstaterenderer .title title="Class BuildThreadStateRenderer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.BuildThreadStateRenderer

::: description
-   

    All Implemented Interfaces:
    :   `MultiStateRenderer`

    ------------------------------------------------------------------------

        public class BuildThreadStateRenderer
        extends Object
        implements MultiStateRenderer
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                             Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildThreadStateRenderer​(Ansi ansi,                         java.util.function.Function<Long,​String> formatTimeFunction,                         long currentTimeMs,                         int outputMaxColumns,                         long minimumDurationMillis,                         Map<Long,​Optional<? extends LeafEvent>> runningStepsByThread,                         BuildRuleThreadTracker buildRuleThreadTracker)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                               Description
          ------------------------------------------------- ------------------------------------ -------------
          `String`                                          `getExecutorCollectionLabel()`        
          `int`                                             `getExecutorCount()`                  
          `com.google.common.collect.ImmutableList<Long>`   `getSortedIds​(boolean sortByTime)`    
          `String`                                          `renderShortStatus​(long threadId)`    
          `String`                                          `renderStatusLine​(long threadId)`     

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

        []{#<init>(com.facebook.buck.util.Ansi,java.util.function.Function,long,int,long,java.util.Map,com.facebook.buck.event.listener.BuildRuleThreadTracker)}

        -   #### BuildThreadStateRenderer

                public BuildThreadStateRenderer​(Ansi ansi,
                                                java.util.function.Function<Long,​String> formatTimeFunction,
                                                long currentTimeMs,
                                                int outputMaxColumns,
                                                long minimumDurationMillis,
                                                Map<Long,​Optional<? extends LeafEvent>> runningStepsByThread,
                                                BuildRuleThreadTracker buildRuleThreadTracker)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExecutorCollectionLabel()}

        -   #### getExecutorCollectionLabel

            ``` methodSignature
            public String getExecutorCollectionLabel()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutorCollectionLabel` in
                interface `MultiStateRenderer`

        []{#getExecutorCount()}

        -   #### getExecutorCount

            ``` methodSignature
            public int getExecutorCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutorCount` in interface `MultiStateRenderer`

        []{#getSortedIds(boolean)}

        -   #### getSortedIds

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Long> getSortedIds​(boolean sortByTime)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSortedIds` in interface `MultiStateRenderer`

        []{#renderStatusLine(long)}

        -   #### renderStatusLine

            ``` methodSignature
            public String renderStatusLine​(long threadId)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `renderStatusLine` in interface `MultiStateRenderer`

        []{#renderShortStatus(long)}

        -   #### renderShortStatus

            ``` methodSignature
            public String renderShortStatus​(long threadId)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `renderShortStatus` in interface `MultiStateRenderer`
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
