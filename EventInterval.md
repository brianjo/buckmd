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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener.util](package-summary.html)
:::

## Class EventInterval {#class-eventinterval .title title="Class EventInterval"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.util.EventInterval

::: description
-   

    ------------------------------------------------------------------------

        public abstract class EventInterval
        extends Object

    ::: block
    Utility class to help match up start and end events
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `EventInterval()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `finish​(long finish)` |                       |
        | static EventInterval` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getElapsedTimeMs()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getEndTime()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getFinish()`         |                       |
        | bstract OptionalLong` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getStart()`          |                       |
        | bstract OptionalLong` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getStartTime()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isComplete()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isOngoing()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isStarted()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `o                    |                       |
        | static EventInterval` | f​(OptionalLong start, |                       |
        |                       |    OptionalLong end)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `proxy​(long s         | ::: block             |
        | static EventInterval` | tart,      long end)` | Build a proxy event   |
        |                       |                       | pair from a start and |
        |                       |                       | end timestamp         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `start​(long start)`   |                       |
        | static EventInterval` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `EventInterval`       | `withFinish​(l         |                       |
        |                       | ong timestampMillis)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `EventInterval`       | `withStart​(l          |                       |
        |                       | ong timestampMillis)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### EventInterval

                public EventInterval()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getStart()}

        -   #### getStart

            ``` methodSignature
            public abstract OptionalLong getStart()
            ```

        []{#getFinish()}

        -   #### getFinish

            ``` methodSignature
            public abstract OptionalLong getFinish()
            ```

        []{#isStarted()}

        -   #### isStarted

            ``` methodSignature
            public boolean isStarted()
            ```

            [Returns:]{.returnLabel}
            :   true if this event pair has a start.

        []{#isComplete()}

        -   #### isComplete

            ``` methodSignature
            public boolean isComplete()
            ```

            [Returns:]{.returnLabel}
            :   true if this event pair has a start and an end, false
                otherwise.

        []{#isOngoing()}

        -   #### isOngoing

            ``` methodSignature
            public boolean isOngoing()
            ```

            [Returns:]{.returnLabel}
            :   true if this event pair has been started, but has not
                yet been finished.

        []{#getStartTime()}

        -   #### getStartTime

            ``` methodSignature
            public long getStartTime()
            ```

            [Returns:]{.returnLabel}
            :   the start time of this event or -1 if this pair does not
                contain a start

        []{#getEndTime()}

        -   #### getEndTime

            ``` methodSignature
            public long getEndTime()
            ```

            [Returns:]{.returnLabel}
            :   the end time of this event or -1 if this pair does not
                contain an end

        []{#getElapsedTimeMs()}

        -   #### getElapsedTimeMs

            ``` methodSignature
            public long getElapsedTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   the difference between the start and end events in ms if
                this event pair is complete, 0 otherwise.

        []{#proxy(long,long)}

        -   #### proxy

            ``` methodSignature
            public static EventInterval proxy​(long start,
                                              long end)
            ```

            ::: block
            Build a proxy event pair from a start and end timestamp
            :::

            [Parameters:]{.paramLabel}
            :   `start` - the start time of the resulting pair
            :   `end` - the end time of the resulting pair

            [Returns:]{.returnLabel}
            :   an event pair made from two proxy (synthetic) events

        []{#of(java.util.OptionalLong,java.util.OptionalLong)}

        -   #### of

            ``` methodSignature
            public static EventInterval of​(OptionalLong start,
                                           OptionalLong end)
            ```

        []{#start(long)}

        -   #### start

            ``` methodSignature
            public static EventInterval start​(long start)
            ```

        []{#finish(long)}

        -   #### finish

            ``` methodSignature
            public static EventInterval finish​(long finish)
            ```

        []{#withStart(long)}

        -   #### withStart

            ``` methodSignature
            public EventInterval withStart​(long timestampMillis)
            ```

        []{#withFinish(long)}

        -   #### withFinish

            ``` methodSignature
            public EventInterval withFinish​(long timestampMillis)
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
