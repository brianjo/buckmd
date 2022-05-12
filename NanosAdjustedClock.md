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

## Class NanosAdjustedClock {#class-nanosadjustedclock .title title="Class NanosAdjustedClock"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.timing.DefaultClock](DefaultClock.html "class in com.facebook.buck.util.timing")

    -   -   com.facebook.buck.util.timing.NanosAdjustedClock

::: description
-   

    All Implemented Interfaces:
    :   `Clock`

    ------------------------------------------------------------------------

        public class NanosAdjustedClock
        extends DefaultClock

    ::: block
    [`Clock`](Clock.html "interface in com.facebook.buck.util.timing")
    implementation that invokes the
    [`System`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true "class or interface in java.lang"){.externalLink}
    calls, adjusted to use the given nanos epoch.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                            Description
          -------------------------------------------------------------------------------------- -------------
          `NanosAdjustedClock​(long nanosEpoch)`                                                   
          `NanosAdjustedClock​(long nanosEpoch,                   boolean enableThreadCpuTime)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method         Description
          ------------------- -------------- -------------
          `long`              `nanoTime()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.timing.DefaultClock}

            ### Methods inherited from class com.facebook.buck.util.timing.[DefaultClock](DefaultClock.html "class in com.facebook.buck.util.timing")

            `currentTimeMillis, threadUserNanoTime`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(long)}

        -   #### NanosAdjustedClock

                public NanosAdjustedClock​(long nanosEpoch)

        []{#<init>(long,boolean)}

        -   #### NanosAdjustedClock

                public NanosAdjustedClock​(long nanosEpoch,
                                          boolean enableThreadCpuTime)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#nanoTime()}

        -   #### nanoTime

            ``` methodSignature
            public long nanoTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `nanoTime` in interface `Clock`

            [Overrides:]{.overrideSpecifyLabel}
            :   `nanoTime` in class `DefaultClock`

            [See Also:]{.seeLabel}
            :   [`System.nanoTime()`](http://docs.oracle.com/javase/7/docs/api/java/lang/System.html?is-external=true#nanoTime() "class or interface in java.lang"){.externalLink}
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
