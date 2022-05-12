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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.tools](package-summary.html)
:::

## Interface IsolationChecker.FailureReporter {#interface-isolationchecker.failurereporter .title title="Interface IsolationChecker.FailureReporter"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [IsolationChecker](IsolationChecker.html "class in com.facebook.buck.rules.modern.tools")

    ------------------------------------------------------------------------

        public static interface IsolationChecker.FailureReporter

    ::: block
    IsolationChecker reports diagnostics through a FailureReporter.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `reportAbsolutePath​(BuildRule instance,                   String crumbs,                   Path path)`                                 
          `void`              `reportNotMbr​(BuildRule instance)`                                                                                                     
          `void`              `reportSerializationFailure​(BuildRule instance,                           String crumbs,                           String message)`    
          `void`              `reportSuccess​(BuildRule instance)`                                                                                                    

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

        []{#reportNotMbr(com.facebook.buck.core.rules.BuildRule)}

        -   #### reportNotMbr

            ``` methodSignature
            void reportNotMbr​(BuildRule instance)
            ```

        []{#reportSerializationFailure(com.facebook.buck.core.rules.BuildRule,java.lang.String,java.lang.String)}

        -   #### reportSerializationFailure

            ``` methodSignature
            void reportSerializationFailure​(BuildRule instance,
                                            String crumbs,
                                            String message)
            ```

        []{#reportAbsolutePath(com.facebook.buck.core.rules.BuildRule,java.lang.String,java.nio.file.Path)}

        -   #### reportAbsolutePath

            ``` methodSignature
            void reportAbsolutePath​(BuildRule instance,
                                    String crumbs,
                                    Path path)
            ```

        []{#reportSuccess(com.facebook.buck.core.rules.BuildRule)}

        -   #### reportSuccess

            ``` methodSignature
            void reportSuccess​(BuildRule instance)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
