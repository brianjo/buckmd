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
[Package]{.packageLabelInType} [com.facebook.buck.counters](package-summary.html)
:::

## Class IntegerCounter {#class-integercounter .title title="Class IntegerCounter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.counters.Counter](Counter.html "class in com.facebook.buck.counters")

    -   -   com.facebook.buck.counters.IntegerCounter

::: description
-   

    ------------------------------------------------------------------------

        public class IntegerCounter
        extends Counter
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `IntegerCounter​(String category,               String name,               com.google.common.collect.ImmutableMap<String,​String> tags)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optio                | `flush()`             | ::: block             |
        | nal<CounterSnapshot>` |                       | If the counter has no |
        |                       |                       | data, returns an      |
        |                       |                       | absent value.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `get()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `inc()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `inc​(long delta)`     |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.counters.Counter}

            ### Methods inherited from class com.facebook.buck.counters.[Counter](Counter.html "class in com.facebook.buck.counters")

            `equals, getCategory, getName, getTags, hashCode, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### IntegerCounter

                public IntegerCounter​(String category,
                                      String name,
                                      com.google.common.collect.ImmutableMap<String,​String> tags)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#inc()}

        -   #### inc

            ``` methodSignature
            public void inc()
            ```

        []{#inc(long)}

        -   #### inc

            ``` methodSignature
            public void inc​(long delta)
            ```

        []{#get()}

        -   #### get

            ``` methodSignature
            public long get()
            ```

        []{#flush()}

        -   #### flush

            ``` methodSignature
            public Optional<CounterSnapshot> flush()
            ```

            ::: block
            [Description copied from
            class: `Counter`]{.descfrmTypeLabel}
            :::

            ::: block
            If the counter has no data, returns an absent value.
            Otherwise, creates a snapshot of the current internal state
            of the counter builder, resets the counter, then returns the
            snapshot.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `flush` in class `Counter`
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