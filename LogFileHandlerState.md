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

## Interface LogFileHandlerState {#interface-logfilehandlerstate .title title="Interface LogFileHandlerState"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ThreadIdToCommandIdMapper`

    ------------------------------------------------------------------------

        public interface LogFileHandlerState
        extends ThreadIdToCommandIdMapper
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                           Description
          -------------------- -------------------------------- -------------
          `Iterable<Writer>`   `getWriters​(String commandId)`    

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

        []{#getWriters(java.lang.String)}

        -   #### getWriters

            ``` methodSignature
            Iterable<Writer> getWriters​(@Nullable
                                        String commandId)
            ```

            [Parameters:]{.paramLabel}
            :   `commandId` - If null all available writers will be
                returned.

            [Returns:]{.returnLabel}
            :   Writers related to the argument commandId.
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