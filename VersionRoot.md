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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Interface VersionRoot\<A extends [BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-versionroota-extends-buildrulearg .title title="Interface VersionRoot"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BaseDescription<A>`, `Description<A>`,
        `DescriptionWithTargetGraph<A>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CxxBinaryDescription`, `CxxTestDescription`,
        `DBinaryDescription`, `DTestDescription`, `GenruleDescription`,
        `GoBinaryDescription`, `GoTestDescription`,
        `HaskellBinaryDescription`, `HaskellGhciDescription`,
        `JavaBinaryDescription`, `JavaTestDescription`,
        `LuaBinaryDescription`, `OcamlBinaryDescription`,
        `PythonBinaryDescription`, `PythonTestDescription`,
        `RustBinaryDescription`, `RustTestDescription`

    ------------------------------------------------------------------------

        public interface VersionRoot<A extends BuildRuleArg>
        extends DescriptionWithTargetGraph<A>

    ::: block
    A node which is the root of a version sub-graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                    Description
          ------------------- ------------------------------------------------------------------------- -------------
          `default boolean`   `isVersionRoot​(com.google.common.collect.ImmutableSet<Flavor> flavors)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `createBuildRule, producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isVersionRoot(com.google.common.collect.ImmutableSet)}

        -   #### isVersionRoot

            ``` methodSignature
            default boolean isVersionRoot​(com.google.common.collect.ImmutableSet<Flavor> flavors)
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
