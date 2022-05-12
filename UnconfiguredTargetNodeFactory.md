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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Interface UnconfiguredTargetNodeFactory {#interface-unconfiguredtargetnodefactory .title title="Interface UnconfiguredTargetNodeFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultUnconfiguredTargetNodeFactory`

    ------------------------------------------------------------------------

        public interface UnconfiguredTargetNodeFactory

    ::: block
    Generic factory to create
    [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Un                   | `create​(              | ::: block             |
        | configuredTargetNode` | Cell cell,       Path | Create new            |
        |                       |  buildFile,       Unc | [`UnconfiguredTarge   |
        |                       | onfiguredBuildTarget  | tNode`](../core/model |
        |                       | buildTarget,       De | /targetgraph/raw/Unco |
        |                       | pendencyStack depende | nfiguredTargetNode.ht |
        |                       | ncyStack,       Map<S | ml "interface in com. |
        |                       | tring,​Object> rawNode | facebook.buck.core.mo |
        |                       | ,       Package pkg)` | del.targetgraph.raw") |
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

        []{#create(com.facebook.buck.core.cell.Cell,java.nio.file.Path,com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.core.exceptions.DependencyStack,java.util.Map,com.facebook.buck.core.model.targetgraph.impl.Package)}

        -   #### create

            ``` methodSignature
            UnconfiguredTargetNode create​(Cell cell,
                                          Path buildFile,
                                          UnconfiguredBuildTarget buildTarget,
                                          DependencyStack dependencyStack,
                                          Map<String,​Object> rawNode,
                                          Package pkg)
            ```

            ::: block
            Create new
            [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - object that current build target belongs to
            :   `buildFile` - An absolute path to a build file that has
                the corresponding build target
            :   `buildTarget` - A build target that uniquely identifies
                created
                [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            :   `dependencyStack` -
            :   `rawNode` - Raw attributes that forms the node, a Map
                where a key is attribute name as
            :   `pkg` - Package to apply to this node.
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
