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
[Package]{.packageLabelInType} [com.facebook.buck.json](package-summary.html)
:::

## Interface BuildFilePythonResult {#interface-buildfilepythonresult .title title="Interface BuildFilePythonResult"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface BuildFilePythonResult

    ::: block
    Immutable value type used to hold the parsed and deserialized output
    of `buck.py`.
    {@see BuildFilePythonResultDeserializer} which specializes in
    deserializing this type from JSON.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                                                                                                                                                                            Description
          --------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Map<String,​Object>>`   `getDiagnostics()`                                                                                                                                                                 
          `Optional<String>`                                              `getProfile()`                                                                                                                                                                     
          `com.google.common.collect.ImmutableList<Map<String,​Object>>`   `getValues()`                                                                                                                                                                      
          `static BuildFilePythonResult`                                  `of​(com.google.common.collect.ImmutableList<Map<String,​Object>> values,   com.google.common.collect.ImmutableList<Map<String,​Object>> diagnostics,   Optional<String> profile)`    

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

        []{#getValues()}

        -   #### getValues

            ``` methodSignature
            com.google.common.collect.ImmutableList<Map<String,​Object>> getValues()
            ```

        []{#getDiagnostics()}

        -   #### getDiagnostics

            ``` methodSignature
            com.google.common.collect.ImmutableList<Map<String,​Object>> getDiagnostics()
            ```

        []{#getProfile()}

        -   #### getProfile

            ``` methodSignature
            Optional<String> getProfile()
            ```

        []{#of(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,java.util.Optional)}

        -   #### of

            ``` methodSignature
            static BuildFilePythonResult of​(com.google.common.collect.ImmutableList<Map<String,​Object>> values,
                                            com.google.common.collect.ImmutableList<Map<String,​Object>> diagnostics,
                                            Optional<String> profile)
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
