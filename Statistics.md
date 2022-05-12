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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class Statistics {#class-statistics .title title="Class Statistics"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.Statistics

::: description
-   

    ------------------------------------------------------------------------

        public class Statistics
        extends Object

    ::: block
    A crappy version of
    `org.apache.commons.math3.stat.descriptive.SummaryStatistics`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `Statistics()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `a                    | ::: block             |
        |                       | ddValue​(long millis)` | Add a value to the    |
        |                       |                       | data.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `double`              | `getConfid            | ::: block             |
        |                       | enceIntervalOffset()` | Get the 97.5%         |
        |                       |                       | z-score.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `double`              | `getMean()`           | ::: block             |
        |                       |                       | Get the mean.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getN()`              | ::: block             |
        |                       |                       | Get the count of      |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `double`              | `ge                   | ::: block             |
        |                       | tStandardDeviation()` | Get the standard      |
        |                       |                       | deviation.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `double`              | `getVariance()`       | ::: block             |
        |                       |                       | Get the standard      |
        |                       |                       | deviation.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### Statistics

                public Statistics()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addValue(long)}

        -   #### addValue

            ``` methodSignature
            public void addValue​(long millis)
            ```

            ::: block
            Add a value to the data.
            :::

        []{#getN()}

        -   #### getN

            ``` methodSignature
            public long getN()
            ```

            ::: block
            Get the count of values.
            :::

        []{#getMean()}

        -   #### getMean

            ``` methodSignature
            public double getMean()
            ```

            ::: block
            Get the mean.
            :::

        []{#getVariance()}

        -   #### getVariance

            ``` methodSignature
            public double getVariance()
            ```

            ::: block
            Get the standard deviation.
            :::

        []{#getStandardDeviation()}

        -   #### getStandardDeviation

            ``` methodSignature
            public double getStandardDeviation()
            ```

            ::: block
            Get the standard deviation.
            :::

        []{#getConfidenceIntervalOffset()}

        -   #### getConfidenceIntervalOffset

            ``` methodSignature
            public double getConfidenceIntervalOffset()
            ```

            ::: block
            Get the 97.5% z-score. \[ getMean() - getZScore(),
            getMean() + getZscore()\] gives approximately a nice 95%
            confidence interval for the mean.
            :::
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
