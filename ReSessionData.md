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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event.listener.model](package-summary.html)
:::

## Interface ReSessionData {#interface-resessiondata .title title="Interface ReSessionData"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ReSessionData

    ::: block
    Information specific to Remote Execution.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                                                                                                                    Description
          ------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.facebook.buck.remoteexecution.proto.RESessionID`   `getReSessionId()`                                                                                                                         
          `String`                                                `getReSessionLabel()`                                                                                                                      
          `ModernBuildRuleBuildStrategy`                          `getStrategy()`                                                                                                                            
          `static ReSessionData`                                  `of​(com.facebook.buck.remoteexecution.proto.RESessionID reSessionId,   String reSessionLabel,   ModernBuildRuleBuildStrategy strategy)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getReSessionId()}

        -   #### getReSessionId

            ``` methodSignature
            com.facebook.buck.remoteexecution.proto.RESessionID getReSessionId()
            ```

        []{#getReSessionLabel()}

        -   #### getReSessionLabel

            ``` methodSignature
            String getReSessionLabel()
            ```

        []{#getStrategy()}

        -   #### getStrategy

            ``` methodSignature
            ModernBuildRuleBuildStrategy getStrategy()
            ```

        []{#of(com.facebook.buck.remoteexecution.proto.RESessionID,java.lang.String,com.facebook.buck.rules.modern.config.ModernBuildRuleBuildStrategy)}

        -   #### of

            ``` methodSignature
            static ReSessionData of​(com.facebook.buck.remoteexecution.proto.RESessionID reSessionId,
                                    String reSessionLabel,
                                    ModernBuildRuleBuildStrategy strategy)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
