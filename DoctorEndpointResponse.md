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
[Package]{.packageLabelInType} [com.facebook.buck.doctor.config](package-summary.html)
:::

## Interface DoctorEndpointResponse {#interface-doctorendpointresponse .title title="Interface DoctorEndpointResponse"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface DoctorEndpointResponse
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                                                                         Description
          ------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------- -------------
          `Optional<String>`                                            `getErrorMessage()`                                                                                             
          `com.google.common.collect.ImmutableList<DoctorSuggestion>`   `getSuggestions()`                                                                                              
          `static DoctorEndpointResponse`                               `of​(Optional<String> errorMessage,   com.google.common.collect.ImmutableList<DoctorSuggestion> suggestions)`    

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

        []{#getErrorMessage()}

        -   #### getErrorMessage

            ``` methodSignature
            Optional<String> getErrorMessage()
            ```

        []{#getSuggestions()}

        -   #### getSuggestions

            ``` methodSignature
            com.google.common.collect.ImmutableList<DoctorSuggestion> getSuggestions()
            ```

        []{#of(java.util.Optional,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            static DoctorEndpointResponse of​(Optional<String> errorMessage,
                                             com.google.common.collect.ImmutableList<DoctorSuggestion> suggestions)
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
