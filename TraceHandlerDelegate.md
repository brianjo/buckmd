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

## Class TraceHandlerDelegate {#class-tracehandlerdelegate .title title="Class TraceHandlerDelegate"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.httpserver.TraceHandlerDelegate

::: description
-   

    All Implemented Interfaces:
    :   `TemplateHandlerDelegate`

    ------------------------------------------------------------------------

        public class TraceHandlerDelegate
        extends Object
        implements TemplateHandlerDelegate

    ::: block
    HTTP handler for requests to the `/trace` path.
    :::
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
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTemplateForRequest(org.eclipse.jetty.server.Request)}

        -   #### getTemplateForRequest

            ``` methodSignature
            public String getTemplateForRequest​(org.eclipse.jetty.server.Request baseRequest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTemplateForRequest` in
                interface `TemplateHandlerDelegate`

            [Parameters:]{.paramLabel}
            :   `baseRequest` - Request that will be served by this
                handler. This gives the handler the opportunity to
                return a different template based on the data in the
                request.

        []{#getDataForRequest(org.eclipse.jetty.server.Request)}

        -   #### getDataForRequest

            ``` methodSignature
            @Nullable
            public com.google.common.collect.ImmutableMap<String,​Object> getDataForRequest​(org.eclipse.jetty.server.Request baseRequest)
                                                                                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDataForRequest` in
                interface `TemplateHandlerDelegate`

            [Parameters:]{.paramLabel}
            :   `baseRequest` - Request that will be served by this
                handler.

            [Returns:]{.returnLabel}
            :   Map to populate the template returned by
                [`TemplateHandlerDelegate.getTemplateForRequest(Request)`](TemplateHandlerDelegate.html#getTemplateForRequest(org.eclipse.jetty.server.Request)).
                If the request is malformed, then return `null` in this
                method to indicate an error.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getTemplateGroup()}

        -   #### getTemplateGroup

            ``` methodSignature
            public URL getTemplateGroup()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTemplateGroup` in
                interface `TemplateHandlerDelegate`

            [Returns:]{.returnLabel}
            :   templates that are available as resources relative to
                the implementation\'s class.
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
