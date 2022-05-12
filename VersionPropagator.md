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
-   Method

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

## Interface VersionPropagator\<A extends [BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-versionpropagatora-extends-buildrulearg .title title="Interface VersionPropagator"}
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
    :   `AppleLibraryDescription`, `CgoLibraryDescription`,
        `CxxGenruleDescription`, `CxxLibraryDescription`,
        `CxxLuaExtensionDescription`, `CxxPrecompiledHeaderDescription`,
        `CxxPythonExtensionDescription`, `DLibraryDescription`,
        `GoLibraryDescription`, `HaskellHaddockDescription`,
        `HaskellLibraryDescription`,
        `HaskellPrebuiltLibraryDescription`,
        `JavaAnnotationProcessorDescription`, `JavaLibraryDescription`,
        `JavaTestRunnerDescription`, `LuaLibraryDescription`,
        `OcamlLibraryDescription`, `PrebuiltCxxLibraryDescription`,
        `PrebuiltCxxLibraryGroupDescription`,
        `PrebuiltGoLibraryDescription`, `PrebuiltJarDescription`,
        `PrebuiltOcamlLibraryDescription`,
        `PrebuiltRustLibraryDescription`, `PythonLibraryDescription`,
        `RustLibraryDescription`, `ZipFileDescription`

    ------------------------------------------------------------------------

        public interface VersionPropagator<A extends BuildRuleArg>
        extends DescriptionWithTargetGraph<A>

    ::: block
    A node constitutes the body of a version sub-graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
