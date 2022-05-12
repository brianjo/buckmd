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
[Package]{.packageLabelInType} [com.facebook.buck.util.timing](package-summary.html)
:::

## Class DefaultClock {#class-defaultclock .title title="Class DefaultClock"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.timing.DefaultClock

::: description
-   

    All Implemented Interfaces:
    :   `Clock`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `NanosAdjustedClock`

    ------------------------------------------------------------------------

        public class DefaultClock
        extends Object
        implements Clock

    ::: block
    [`Clock`](Clock.html "interface in com.facebook.buck.util.timing")
    implementation that invokes the
    [`System`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true "class or interface in java.lang"){.externalLink}
    calls.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                   Description
          --------------------------------------------- -------------
          `DefaultClock()`                               
          `DefaultClock​(boolean enableThreadCpuTime)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                Description
          ------------------- ------------------------------------- -------------
          `long`              `currentTimeMillis()`                  
          `long`              `nanoTime()`                           
          `long`              `threadUserNanoTime​(long threadId)`    

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

        []{#<init>()}

        -   #### DefaultClock

                public DefaultClock()

        []{#<init>(boolean)}

        -   #### DefaultClock

                public DefaultClock​(boolean enableThreadCpuTime)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#currentTimeMillis()}

        -   #### currentTimeMillis

            ``` methodSignature
            public long currentTimeMillis()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `currentTimeMillis` in interface `Clock`

            [See Also:]{.seeLabel}
            :   [`System.currentTimeMillis()`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true#currentTimeMillis() "class or interface in java.lang"){.externalLink}

        []{#nanoTime()}

        -   #### nanoTime

            ``` methodSignature
            public long nanoTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `nanoTime` in interface `Clock`

            [See Also:]{.seeLabel}
            :   [`System.nanoTime()`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true#nanoTime() "class or interface in java.lang"){.externalLink}

        []{#threadUserNanoTime(long)}

        -   #### threadUserNanoTime

            ``` methodSignature
            public long threadUserNanoTime​(long threadId)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `threadUserNanoTime` in interface `Clock`

            [See Also:]{.seeLabel}
            :   [`ThreadMXBean.getThreadUserTime(long)`](http://docs.oracle.com/javase/7/docs/api/java/lang/management/ThreadMXBean.html?is-external=true#getThreadUserTime(long) "class or interface in java.lang.management"){.externalLink}
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
