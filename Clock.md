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
[Package]{.packageLabelInType} [com.facebook.buck.util.timing](package-summary.html)
:::

## Interface Clock {#interface-clock .title title="Interface Clock"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultClock`, `NanosAdjustedClock`

    ------------------------------------------------------------------------

        public interface Clock
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                Description
          ------------------- ------------------------------------- -------------
          `long`              `currentTimeMillis()`                  
          `long`              `nanoTime()`                           
          `long`              `threadUserNanoTime​(long threadId)`    

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

        []{#currentTimeMillis()}

        -   #### currentTimeMillis

            ``` methodSignature
            long currentTimeMillis()
            ```

            [See Also:]{.seeLabel}
            :   [`System.currentTimeMillis()`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true#currentTimeMillis() "class or interface in java.lang"){.externalLink}

        []{#nanoTime()}

        -   #### nanoTime

            ``` methodSignature
            long nanoTime()
            ```

            [See Also:]{.seeLabel}
            :   [`System.nanoTime()`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true#nanoTime() "class or interface in java.lang"){.externalLink}

        []{#threadUserNanoTime(long)}

        -   #### threadUserNanoTime

            ``` methodSignature
            long threadUserNanoTime​(long threadId)
            ```

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
