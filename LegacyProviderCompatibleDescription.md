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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface LegacyProviderCompatibleDescription\<T extends [BuildRuleArg](../description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-legacyprovidercompatibledescriptiont-extends-buildrulearg .title title="Interface LegacyProviderCompatibleDescription"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BaseDescription<T>`, `Description<T>`,
        `DescriptionWithTargetGraph<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CsharpLibraryDescription`, `HttpArchiveDescription`,
        `HttpFileDescription`

    ------------------------------------------------------------------------

        public interface LegacyProviderCompatibleDescription<T extends BuildRuleArg>
        extends DescriptionWithTargetGraph<T>

    ::: block
    Marks a
    [`DescriptionWithTargetGraph`](DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")
    as compatible with
    [`Provider`](providers/Provider.html "interface in com.facebook.buck.core.rules.providers")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                                                              Description
          -------------------------- ------------------------------------------------------------------------------------------------------------------- -------------
          `ProviderInfoCollection`   `createProviders​(ProviderCreationContext context,                BuildTarget buildTarget,                T args)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `createBuildRule, producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.description.arg.BuildRuleArg)}
        []{#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T)}

        -   #### createProviders

            ``` methodSignature
            ProviderInfoCollection createProviders​(ProviderCreationContext context,
                                                   BuildTarget buildTarget,
                                                   T args)
            ```

            [Parameters:]{.paramLabel}
            :   `context` - the
                [`ProviderCreationContext`](ProviderCreationContext.html "interface in com.facebook.buck.core.rules")
                that the implementation has access to
            :   `buildTarget` - the current
                [`BuildTarget`](../model/BuildTarget.html "class in com.facebook.buck.core.model"),
                with flavours
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../description/BaseDescription.html#getConstructorArgType())

            [Returns:]{.returnLabel}
            :   the
                [`ProviderInfoCollection`](providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                of this rule.
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
