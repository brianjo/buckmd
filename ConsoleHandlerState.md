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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Interface ConsoleHandlerState {#interface-consolehandlerstate .title title="Interface ConsoleHandlerState"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ThreadIdToCommandIdMapper`

    ------------------------------------------------------------------------

        public interface ConsoleHandlerState
        extends ThreadIdToCommandIdMapper

    ::: block
    How the ConsoleHandler is supposed to behave for a particular
    thread. Maintained globally by
    [`GlobalStateManager`](GlobalStateManager.html "class in com.facebook.buck.log").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                      Description
          --------------------- ------------------------------ -------------
          `static interface `   `ConsoleHandlerState.Writer`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                        Method                            Description
          ---------------------------------------- --------------------------------- -------------
          `Iterable<ConsoleHandlerState.Writer>`   `getAllAvailableWriters()`         
          `Level`                                  `getLogLevel​(String commandId)`    
          `ConsoleHandlerState.Writer`             `getWriter​(String commandId)`      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.concurrent.ThreadIdToCommandIdMapper}

            ### Methods inherited from interface com.facebook.buck.util.concurrent.[ThreadIdToCommandIdMapper](../util/concurrent/ThreadIdToCommandIdMapper.html "interface in com.facebook.buck.util.concurrent")

            `threadIdToCommandId`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLogLevel(java.lang.String)}

        -   #### getLogLevel

            ``` methodSignature
            Level getLogLevel​(String commandId)
            ```

        []{#getWriter(java.lang.String)}

        -   #### getWriter

            ``` methodSignature
            ConsoleHandlerState.Writer getWriter​(String commandId)
            ```

        []{#getAllAvailableWriters()}

        -   #### getAllAvailableWriters

            ``` methodSignature
            Iterable<ConsoleHandlerState.Writer> getAllAvailableWriters()
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
-   [Nested](#nested.class.summary) \| 
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
