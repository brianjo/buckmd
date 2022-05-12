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

## Interface ProviderCreationContext {#interface-providercreationcontext .title title="Interface ProviderCreationContext"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ProviderCreationContext

    ::: block
    The context given to
    [`LegacyProviderCompatibleDescription.createProviders(ProviderCreationContext, BuildTarget,  BuildRuleArg)`](LegacyProviderCompatibleDescription.html#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T)).
    This is to be a subset of
    [`BuildRuleCreationContextWithTargetGraph`](BuildRuleCreationContextWithTargetGraph.html "interface in com.facebook.buck.core.rules"),
    plus the
    [`ProviderInfoCollection`](providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
    of all the dependencies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                              Method                                                                                                                  Description
          ------------------------------------------------------------------------------ ----------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection>`   `dependencies()`                                                                                                         
          `ProjectFilesystem`                                                            `getProjectFilesystem()`                                                                                                 
          `static ProviderCreationContext`                                               `of​(Map<? extends BuildTarget,​? extends ProviderInfoCollection> dependencies,   ProjectFilesystem projectFilesystem)`    

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

        []{#dependencies()}

        -   #### dependencies

            ``` methodSignature
            com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> dependencies()
            ```

            [Returns:]{.returnLabel}
            :   [`ProviderInfoCollection`](providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                of the parse time dependencies

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            ProjectFilesystem getProjectFilesystem()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
                for the rule

        []{#of(java.util.Map,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### of

            ``` methodSignature
            static ProviderCreationContext of​(Map<? extends BuildTarget,​? extends ProviderInfoCollection> dependencies,
                                              ProjectFilesystem projectFilesystem)
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
