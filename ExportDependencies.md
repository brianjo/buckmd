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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface ExportDependencies {#interface-exportdependencies .title title="Interface ExportDependencies"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `DefaultJavaLibrary`,
        `JavaTest`, `JavaTestX`, `PrebuiltJar`, `RobolectricTest`,
        `RobolectricTestX`

    ------------------------------------------------------------------------

        public interface ExportDependencies
        extends BuildRule

    ::: block
    [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
    that can export a subset of it\'s dependencies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                        Description
          ------------------------ ----------------------------- -------------
          `SortedSet<BuildRule>`   `getExportedDeps()`            
          `SortedSet<BuildRule>`   `getExportedProvidedDeps()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            SortedSet<BuildRule> getExportedDeps()
            ```

        []{#getExportedProvidedDeps()}

        -   #### getExportedProvidedDeps

            ``` methodSignature
            SortedSet<BuildRule> getExportedProvidedDeps()
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