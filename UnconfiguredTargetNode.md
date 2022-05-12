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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.raw](package-summary.html)
:::

## Interface UnconfiguredTargetNode {#interface-unconfiguredtargetnode .title title="Interface UnconfiguredTargetNode"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ComputeResult`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ImmutableUnconfiguredTargetNode`

    ------------------------------------------------------------------------

        public interface UnconfiguredTargetNode
        extends ComputeResult

    ::: block
    A target node with attributes kept in a map as oppose to in a
    structured object like in
    [`TargetNode`](../TargetNode.html "interface in com.facebook.buck.core.model.targetgraph").
    The attributes are coerced from raw data produced by build file
    parser, but they are not stored in a structured object as in
    [`TargetNode`](../TargetNode.html "interface in com.facebook.buck.core.model.targetgraph").

    The main purpose of having such nodes is to perform additional
    processing before storing them in a structured constructor
    arguments.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.c         | `getAttributes()`     | ::: block             |
        | ommon.collect.Immutab |                       | Attributes of this    |
        | leMap<String,​Object>` |                       | node coerced to the   |
        |                       |                       | types declared in     |
        |                       |                       | constructor           |
        |                       |                       | arguments.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `getBuildTarget()`    | ::: block             |
        | onfiguredBuildTarget` |                       | Build target of this  |
        |                       |                       | node.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | List of targets from  |
        | ct.ImmutableList<Unco |                       | `compatible_with`     |
        | nfiguredBuildTarget>` |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | Value of              |
        |                       |                       | `def                  |
        |                       |                       | ault_target_platform` |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RuleType`            | `getRuleType()`       | ::: block             |
        |                       |                       | The type of a rule.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `get                  | ::: block             |
        | n.collect.ImmutableSe | VisibilityPatterns()` | List of patterns from |
        | t<VisibilityPattern>` |                       | `visibility`          |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `get                  | ::: block             |
        | n.collect.ImmutableSe | WithinViewPatterns()` | List of patterns from |
        | t<VisibilityPattern>` |                       | `within_view`         |
        |                       |                       | attribute.            |
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

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            UnconfiguredBuildTarget getBuildTarget()
            ```

            ::: block
            Build target of this node.
            :::

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            RuleType getRuleType()
            ```

            ::: block
            The type of a rule.
            :::

        []{#getAttributes()}

        -   #### getAttributes

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​Object> getAttributes()
            ```

            ::: block
            Attributes of this node coerced to the types declared in
            constructor arguments.
            Note that some of these attributes may require additional
            processing before they can be stored in a constructor
            argument. For example, selectable arguments need to be
            resolved first.
            :::

        []{#getVisibilityPatterns()}

        -   #### getVisibilityPatterns

            ``` methodSignature
            com.google.common.collect.ImmutableSet<VisibilityPattern> getVisibilityPatterns()
            ```

            ::: block
            List of patterns from `visibility` attribute.
            :::

        []{#getWithinViewPatterns()}

        -   #### getWithinViewPatterns

            ``` methodSignature
            com.google.common.collect.ImmutableSet<VisibilityPattern> getWithinViewPatterns()
            ```

            ::: block
            List of patterns from `within_view` attribute.
            :::

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            Value of `default_target_platform` attribute. Note this
            attribute only exists for build targets.
            :::

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            List of targets from `compatible_with` attribute. Note
            method exists for all rules, while `compatible_with` can be
            defined only for build rules.
            :::
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
