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
[Package]{.packageLabelInType} [com.facebook.buck.io.watchman](package-summary.html)
:::

## Class WatchmanDiagnosticEventListener {#class-watchmandiagnosticeventlistener .title title="Class WatchmanDiagnosticEventListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.watchman.WatchmanDiagnosticEventListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        @ThreadSafe
        public class WatchmanDiagnosticEventListener
        extends Object
        implements BuckEventListener

    ::: block
    Deduplicating event bus listener that outputs deduplicated messages
    over the given event bus.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WatchmanDiagnosticEventListener​(BuckEventBus outputEventBus)`                                                                            
          `WatchmanDiagnosticEventListener​(BuckEventBus outputEventBus,                                Set<WatchmanDiagnostic> diagnosticCache)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                     Description
          ------------------- ------------------------------------------ -------------
          `void`              `onEvent​(WatchmanDiagnosticEvent event)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEventListener}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEventListener](../../event/BuckEventListener.html "interface in com.facebook.buck.event")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.BuckEventBus)}

        -   #### WatchmanDiagnosticEventListener

                public WatchmanDiagnosticEventListener​(BuckEventBus outputEventBus)

        []{#<init>(com.facebook.buck.event.BuckEventBus,java.util.Set)}

        -   #### WatchmanDiagnosticEventListener

                public WatchmanDiagnosticEventListener​(BuckEventBus outputEventBus,
                                                       Set<WatchmanDiagnostic> diagnosticCache)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onEvent(com.facebook.buck.io.watchman.WatchmanDiagnosticEvent)}

        -   #### onEvent

            ``` methodSignature
            public void onEvent​(WatchmanDiagnosticEvent event)
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
