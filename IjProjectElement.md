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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Interface IjProjectElement {#interface-ijprojectelement .title title="Interface IjProjectElement"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `IjLibrary`, `IjModule`

    ------------------------------------------------------------------------

        public interface IjProjectElement

    ::: block
    Common interface shared between
    [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")
    and
    [`IjLibrary`](IjLibrary.html "class in com.facebook.buck.features.project.intellij.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                                                                                           Description
          ------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------- -------------
          `void`                                                  `addAsDependency​(DependencyType dependencyType,                IjDependencyListBuilder dependencyListBuilder)`    
          `String`                                                `getName()`                                                                                                       
          `com.google.common.collect.ImmutableSet<BuildTarget>`   `getTargets()`                                                                                                    

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

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

            [Returns:]{.returnLabel}
            :   unique string identifying the element. This will be used
                by modules to refer to it.

        []{#getTargets()}

        -   #### getTargets

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildTarget> getTargets()
            ```

            [Returns:]{.returnLabel}
            :   set of targets this element corresponds to in the
                IntelliJ project.

        []{#addAsDependency(com.facebook.buck.features.project.intellij.model.DependencyType,com.facebook.buck.features.project.intellij.IjDependencyListBuilder)}

        -   #### addAsDependency

            ``` methodSignature
            void addAsDependency​(DependencyType dependencyType,
                                 IjDependencyListBuilder dependencyListBuilder)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
