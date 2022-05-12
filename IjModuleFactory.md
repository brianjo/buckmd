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

## Interface IjModuleFactory {#interface-ijmodulefactory .title title="Interface IjModuleFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultIjModuleFactory`

    ------------------------------------------------------------------------

        public interface IjModuleFactory

    ::: block
    Builds
    [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")s
    out of
    [`TargetNode`](../../../../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `IjModule`            | `createModule​(Pat     | ::: block             |
        |                       | h moduleBasePath,     | Create an             |
        |                       |          com.google.c | [`Ij                  |
        |                       | ommon.collect.Immutab | Module`](IjModule.htm |
        |                       | leSet<TargetNode> tar | l "class in com.faceb |
        |                       | getNodes,             | ook.buck.features.pro |
        |                       |  Set<Path> excludes)` | ject.intellij.model") |
        |                       |                       | form the supplied     |
        |                       |                       | parameters.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#createModule(java.nio.file.Path,com.google.common.collect.ImmutableSet,java.util.Set)}

        -   #### createModule

            ``` methodSignature
            IjModule createModule​(Path moduleBasePath,
                                  com.google.common.collect.ImmutableSet<TargetNode> targetNodes,
                                  Set<Path> excludes)
            ```

            ::: block
            Create an
            [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")
            form the supplied parameters.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleBasePath` - the top-most directory the module is
                responsible for.
            :   `targetNodes` - set of nodes the module is to be created
                from.

            [Returns:]{.returnLabel}
            :   nice shiny new module.
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
