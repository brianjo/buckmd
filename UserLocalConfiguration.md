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

## Interface UserLocalConfiguration {#interface-userlocalconfiguration .title title="Interface UserLocalConfiguration"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface UserLocalConfiguration
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                          Method                                                                                                                                          Description
          -------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableMap<String,​String>`                    `getConfigOverrides()`                                                                                                                           
          `com.google.common.collect.ImmutableMap<Path,​String>`                      `getLocalConfigsContents()`                                                                                                                      
          `boolean`                                                                  `isNoBuckCheckPresent()`                                                                                                                         
          `static com.facebook.buck.doctor.config.ImmutableUserLocalConfiguration`   `of​(boolean noBuckCheckPresent,   Map<? extends Path,​? extends String> localConfigsContents,   Map<String,​? extends String> configOverrides)`    

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

        []{#isNoBuckCheckPresent()}

        -   #### isNoBuckCheckPresent

            ``` methodSignature
            boolean isNoBuckCheckPresent()
            ```

        []{#getLocalConfigsContents()}

        -   #### getLocalConfigsContents

            ``` methodSignature
            com.google.common.collect.ImmutableMap<Path,​String> getLocalConfigsContents()
            ```

        []{#getConfigOverrides()}

        -   #### getConfigOverrides

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getConfigOverrides()
            ```

        []{#of(boolean,java.util.Map,java.util.Map)}

        -   #### of

            ``` methodSignature
            static com.facebook.buck.doctor.config.ImmutableUserLocalConfiguration of​(boolean noBuckCheckPresent,
                                                                                      Map<? extends Path,​? extends String> localConfigsContents,
                                                                                      Map<String,​? extends String> configOverrides)
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
