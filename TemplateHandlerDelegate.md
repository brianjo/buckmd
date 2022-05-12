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
[Package]{.packageLabelInType} [com.facebook.buck.httpserver](package-summary.html)
:::

## Interface TemplateHandlerDelegate {#interface-templatehandlerdelegate .title title="Interface TemplateHandlerDelegate"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TraceHandlerDelegate`, `TracesHandlerDelegate`

    ------------------------------------------------------------------------

        public interface TemplateHandlerDelegate
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                  Description
          --------------------------------------------------------- ----------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableMap<String,​Object>`   `getDataForRequest​(org.eclipse.jetty.server.Request baseRequest)`        
          `String`                                                  `getTemplateForRequest​(org.eclipse.jetty.server.Request baseRequest)`    
          `URL`                                                     `getTemplateGroup()`                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTemplateGroup()}

        -   #### getTemplateGroup

            ``` methodSignature
            URL getTemplateGroup()
            ```

            [Returns:]{.returnLabel}
            :   templates that are available as resources relative to
                the implementation\'s class.

        []{#getTemplateForRequest(org.eclipse.jetty.server.Request)}

        -   #### getTemplateForRequest

            ``` methodSignature
            String getTemplateForRequest​(org.eclipse.jetty.server.Request baseRequest)
            ```

            [Parameters:]{.paramLabel}
            :   `baseRequest` - Request that will be served by this
                handler. This gives the handler the opportunity to
                return a different template based on the data in the
                request.

        []{#getDataForRequest(org.eclipse.jetty.server.Request)}

        -   #### getDataForRequest

            ``` methodSignature
            @Nullable
            com.google.common.collect.ImmutableMap<String,​Object> getDataForRequest​(org.eclipse.jetty.server.Request baseRequest)
                                                                                   throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `baseRequest` - Request that will be served by this
                handler.

            [Returns:]{.returnLabel}
            :   Map to populate the template returned by
                [`getTemplateForRequest(Request)`](#getTemplateForRequest(org.eclipse.jetty.server.Request)).
                If the request is malformed, then return `null` in this
                method to indicate an error.

            [Throws:]{.throwsLabel}
            :   `IOException`
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
