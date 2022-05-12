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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.stats](package-summary.html)
:::

## Class BuildRuleDurationTracker {#class-buildruledurationtracker .title title="Class BuildRuleDurationTracker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.stats.BuildRuleDurationTracker

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRuleDurationTracker
        extends Object

    ::: block
    Tracks the total duration of work spent on each build rule.
    Computation associated with build rules are broken into several
    phases. Those phases are invoked from various places in
    [`CachingBuildEngine`](../engine/impl/CachingBuildEngine.html "class in com.facebook.buck.core.build.engine.impl")
    at various times and on various threads. In order to track the total
    duration of all of those phases combined we need some central store,
    i.e. this class.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `BuildRuleDurationTracker()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ClockDuration`       | `do                   |                       |
        |                       | Beginning​(BuildRule r |                       |
        |                       | ule,            long  |                       |
        |                       | wallMillisTime,       |                       |
        |                       |       long nanoTime)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ClockDuration`       | `doEnding​(            |                       |
        |                       | BuildRule rule,       |                       |
        |                       |    long wallMillisTim |                       |
        |                       | e,         long nanoT |                       |
        |                       | ime,         long thr |                       |
        |                       | eadUserNanoDuration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | setDuration​(BuildRule | This method should    |
        |                       |  rule,            Clo | only be used for      |
        |                       | ckDuration duration)` | testing.              |
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

        -   #### BuildRuleDurationTracker

                public BuildRuleDurationTracker()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setDuration(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.util.timing.ClockDuration)}

        -   #### setDuration

            ``` methodSignature
            public void setDuration​(BuildRule rule,
                                    ClockDuration duration)
            ```

            ::: block
            This method should only be used for testing.
            :::

        []{#doBeginning(com.facebook.buck.core.rules.BuildRule,long,long)}

        -   #### doBeginning

            ``` methodSignature
            public ClockDuration doBeginning​(BuildRule rule,
                                             long wallMillisTime,
                                             long nanoTime)
            ```

        []{#doEnding(com.facebook.buck.core.rules.BuildRule,long,long,long)}

        -   #### doEnding

            ``` methodSignature
            public ClockDuration doEnding​(BuildRule rule,
                                          long wallMillisTime,
                                          long nanoTime,
                                          long threadUserNanoDuration)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
