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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function](package-summary.html)
:::

## Interface SkylarkRuleFunctionsApi {#interface-skylarkrulefunctionsapi .title title="Interface SkylarkRuleFunctionsApi"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `SkylarkRuleFunctions`

    ------------------------------------------------------------------------

        public interface SkylarkRuleFunctionsApi

    ::: block
    Interface for a global Skylark library containing rule-related
    helper and registration functions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                               Method                                                                                                                                                                                                                                                                                                                                                                                    Description
          ----------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.devtools.build.lib.cmdline.Label`   `label​(String labelString,      com.google.devtools.build.lib.events.Location loc,      com.google.devtools.build.lib.syntax.Environment env,      com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)`                                                                                                                                                                
          `UserDefinedProvider`                           `provider​(String doc,         Object fields,         com.google.devtools.build.lib.events.Location location)`                                                                                                                                                                                                                                                                              
          `SkylarkUserDefinedRule`                        `rule​(com.google.devtools.build.lib.syntax.BaseFunction implementation,     com.google.devtools.build.lib.syntax.SkylarkDict<String,​AttributeHolder> attrs,     boolean executable,     boolean test,     com.google.devtools.build.lib.events.Location loc,     com.google.devtools.build.lib.syntax.FuncallExpression ast,     com.google.devtools.build.lib.syntax.Environment env)`    

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

        []{#label(java.lang.String,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.syntax.Environment,com.google.devtools.build.lib.skylarkinterface.StarlarkContext)}

        -   #### label

            ``` methodSignature
            com.google.devtools.build.lib.cmdline.Label label​(String labelString,
                                                              com.google.devtools.build.lib.events.Location loc,
                                                              com.google.devtools.build.lib.syntax.Environment env,
                                                              com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)
                                                       throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#rule(com.google.devtools.build.lib.syntax.BaseFunction,com.google.devtools.build.lib.syntax.SkylarkDict,boolean,boolean,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### rule

            ``` methodSignature
            SkylarkUserDefinedRule rule​(com.google.devtools.build.lib.syntax.BaseFunction implementation,
                                        com.google.devtools.build.lib.syntax.SkylarkDict<String,​AttributeHolder> attrs,
                                        boolean executable,
                                        boolean test,
                                        com.google.devtools.build.lib.events.Location loc,
                                        com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                        com.google.devtools.build.lib.syntax.Environment env)
                                 throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#provider(java.lang.String,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### provider

            ``` methodSignature
            UserDefinedProvider provider​(String doc,
                                         Object fields,
                                         com.google.devtools.build.lib.events.Location location)
                                  throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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
