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
-   [Nested](#nested.class.summary) \| 
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

## Class LeafEvents {#class-leafevents .title title="Class LeafEvents"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.LeafEvents

::: description
-   

    ------------------------------------------------------------------------

        public class LeafEvents
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                          Description
          ------------------- ------------------------------ -------------
          `static class `     `LeafEvents.SimpleLeafEvent`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `LeafEvents()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Scope`        | `scope​(Buc            | ::: block             |
        |                       | kEventBus eventBus,   | Creates a simple      |
        |                       |     String category)` | scoped leaf event     |
        |                       |                       | that will be logged   |
        |                       |                       | to superconsole,      |
        |                       |                       | chrome traces, etc.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Scope`        | `scope​(BuckEventBus   |                       |
        |                       | eventBus,      String |                       |
        |                       |  category,      boole |                       |
        |                       | an logToChromeTrace)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### LeafEvents

                public LeafEvents()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#scope(com.facebook.buck.event.BuckEventBus,java.lang.String)}

        -   #### scope

            ``` methodSignature
            public static Scope scope​(BuckEventBus eventBus,
                                      String category)
            ```

            ::: block
            Creates a simple scoped leaf event that will be logged to
            superconsole, chrome traces, etc.
            :::

        []{#scope(com.facebook.buck.event.BuckEventBus,java.lang.String,boolean)}

        -   #### scope

            ``` methodSignature
            public static Scope scope​(BuckEventBus eventBus,
                                      String category,
                                      boolean logToChromeTrace)
            ```

            [Parameters:]{.paramLabel}

            `eventBus` -

            `category` - the name of the category.

            `logToChromeTrace` - if it should be logged to the
            ChromeTrace or not.

            [Returns:]{.returnLabel}
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
-   [Nested](#nested.class.summary) \| 
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
