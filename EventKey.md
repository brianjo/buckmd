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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class EventKey {#class-eventkey .title title="Class EventKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.EventKey

::: description
-   

    ------------------------------------------------------------------------

        public abstract class EventKey
        extends Object

    ::: block
    Used to associate sets of
    [`BuckEvent`](BuckEvent.html "interface in com.facebook.buck.event")s
    with each other. The keys are only considered unique in the scope of
    the same type of
    [`BuckEvent`](BuckEvent.html "interface in com.facebook.buck.event").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `EventKey()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract long`       | `getValue()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static EventKey`     | `of​(long value)`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `setSequenceValu      |                       |
        |                       | eForTest​(long value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static EventKey`     | `slowValueKe          | ::: block             |
        |                       | y​(Object... objects)` | Prefer calling        |
        |                       |                       | chain(started) in the |
        |                       |                       | \@{link BuckEvent}    |
        |                       |                       | over the use of this  |
        |                       |                       | method.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static EventKey`     | `unique()`            |                       |
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

        -   #### EventKey

                public EventKey()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValue()}

        -   #### getValue

            ``` methodSignature
            public abstract long getValue()
            ```

        []{#setSequenceValueForTest(long)}

        -   #### setSequenceValueForTest

            ``` methodSignature
            public static void setSequenceValueForTest​(long value)
            ```

        []{#unique()}

        -   #### unique

            ``` methodSignature
            public static EventKey unique()
            ```

            [Returns:]{.returnLabel}
            :   an EventKey unique to the current process.

        []{#slowValueKey(java.lang.Object...)}

        -   #### slowValueKey

            ``` methodSignature
            public static EventKey slowValueKey​(Object... objects)
            ```

            ::: block
            Prefer calling chain(started) in the \@{link BuckEvent} over
            the use of this method.
            This variant of the method creates a key based on the set of
            supplied inputs. This is useful in situations where a key
            with the same identity must be created multiple times and
            the corresponding start event is not available.
            :::

            [Parameters:]{.paramLabel}
            :   `objects` - objects which supply the identity of the
                key.
                [`Object.toString()`](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true#toString() "class or interface in java.lang"){.externalLink}
                will be called on every instance and the result will be
                used to calculate the key.

            [Returns:]{.returnLabel}
            :   EventKey with the identity of the supplied objects.

        []{#of(long)}

        -   #### of

            ``` methodSignature
            public static EventKey of​(long value)
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
