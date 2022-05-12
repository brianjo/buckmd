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

## Class TimeCostEntry\<T extends [BuckEvent](../BuckEvent.html "interface in com.facebook.buck.event")\> {#class-timecostentryt-extends-buckevent .title title="Class TimeCostEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.TimeCostEntry\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class TimeCostEntry<T extends BuckEvent>
        extends Object

    ::: block
    Data class for storing the amortized time and total time of a
    start/finished event pair.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `TimeCostEntry​(T startEvent)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                       Description
          ------------------- ------------------------------------------------------------ -------------
          `long`              `getAmortizedNanoTime()`                                      
          `T`                 `getFinishEvent()`                                            
          `T`                 `getStartEvent()`                                             
          `long`              `getTotalNanoTime()`                                          
          `long`              `getTotalThreadUserNanoTime()`                                
          `void`              `incrementAmortizedNanoTime​(long nanoIncrement)`              
          `void`              `setFinishEvent​(T finishEvent)`                               
          `void`              `setTotalNanoTime​(long totalNanoTime)`                        
          `void`              `setTotalThreadUserNanoTime​(long totalThreadUserNanoTime)`    

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

        []{#<init>(com.facebook.buck.event.BuckEvent)} []{#<init>(T)}

        -   #### TimeCostEntry

                public TimeCostEntry​(T startEvent)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFinishEvent()}

        -   #### getFinishEvent

            ``` methodSignature
            public T getFinishEvent()
            ```

        []{#setFinishEvent(com.facebook.buck.event.BuckEvent)}
        []{#setFinishEvent(T)}

        -   #### setFinishEvent

            ``` methodSignature
            public void setFinishEvent​(T finishEvent)
            ```

        []{#incrementAmortizedNanoTime(long)}

        -   #### incrementAmortizedNanoTime

            ``` methodSignature
            public void incrementAmortizedNanoTime​(long nanoIncrement)
            ```

        []{#setTotalNanoTime(long)}

        -   #### setTotalNanoTime

            ``` methodSignature
            public void setTotalNanoTime​(long totalNanoTime)
            ```

        []{#setTotalThreadUserNanoTime(long)}

        -   #### setTotalThreadUserNanoTime

            ``` methodSignature
            public void setTotalThreadUserNanoTime​(long totalThreadUserNanoTime)
            ```

        []{#getStartEvent()}

        -   #### getStartEvent

            ``` methodSignature
            public T getStartEvent()
            ```

        []{#getAmortizedNanoTime()}

        -   #### getAmortizedNanoTime

            ``` methodSignature
            public long getAmortizedNanoTime()
            ```

        []{#getTotalNanoTime()}

        -   #### getTotalNanoTime

            ``` methodSignature
            public long getTotalNanoTime()
            ```

        []{#getTotalThreadUserNanoTime()}

        -   #### getTotalThreadUserNanoTime

            ``` methodSignature
            public long getTotalThreadUserNanoTime()
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
