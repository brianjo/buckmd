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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.arg](package-summary.html)
:::

## Interface HasDepsQuery {#interface-hasdepsquery .title title="Interface HasDepsQuery"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `HasDeclaredDeps`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AndroidLibraryDescription.CoreArg`,
        `CxxBinaryDescription.CommonArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`, `AndroidLibraryDescriptionArg`,
        `CgoLibraryDescriptionArg`, `CxxBinaryDescriptionArg`,
        `CxxTestDescriptionArg`, `HalideLibraryDescriptionArg`,
        `HaskellBinaryDescriptionArg`, `HaskellGhciDescriptionArg`,
        `HaskellHaddockDescriptionArg`, `JsLibraryDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasDepsQuery
        extends HasDeclaredDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                         Description
          ------------------- ------------------------------ -------------
          `Optional<Query>`   `getDepsQuery()`                
          `HasDepsQuery`      `withDepsQuery​(Query query)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDeclaredDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDeclaredDeps](HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")

            `getDeps`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDepsQuery()}

        -   #### getDepsQuery

            ``` methodSignature
            Optional<Query> getDepsQuery()
            ```

        []{#withDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### withDepsQuery

            ``` methodSignature
            HasDepsQuery withDepsQuery​(Query query)
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
