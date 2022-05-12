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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Class MergedTargetNode {#class-mergedtargetnode .title title="Class MergedTargetNode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.MergedTargetNode

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<MergedTargetNode>`

    ------------------------------------------------------------------------

        public class MergedTargetNode
        extends Object
        implements Comparable<MergedTargetNode>

    ::: block
    A set of target nodes with the same unconfigured build target.
    This utility exists to support legacy configured `buck query`, and
    should not be used for anything else.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareTo​(Me         |                       |
        |                       | rgedTargetNode that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<?>`       | `getAnyNode()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `getBuildTarget()`    |                       |
        | nflavoredBuildTarget` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getNodes()`          |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eList<TargetNode<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleType`            | `getRuleType()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getTa                |                       |
        | collect.ImmutableSet< | rgetConfigurations()` |                       |
        | TargetConfiguration>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `gro                  | ::: block             |
        | atic com.google.commo | up​(Collection<TargetN | Group targets by      |
        | n.collect.ImmutableMa | ode<?>> targetNodes)` | unflavored target.    |
        | p<UnflavoredBuildTarg |                       | :::                   |
        | et,​MergedTargetNode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNodes()}

        -   #### getNodes

            ``` methodSignature
            public com.google.common.collect.ImmutableList<TargetNode<?>> getNodes()
            ```

        []{#getAnyNode()}

        -   #### getAnyNode

            ``` methodSignature
            public TargetNode<?> getAnyNode()
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public UnflavoredBuildTarget getBuildTarget()
            ```

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            public RuleType getRuleType()
            ```

        []{#group(java.util.Collection)}

        -   #### group

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<UnflavoredBuildTarget,​MergedTargetNode> group​(Collection<TargetNode<?>> targetNodes)
            ```

            ::: block
            Group targets by unflavored target.
            :::

        []{#getTargetConfigurations()}

        -   #### getTargetConfigurations

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<TargetConfiguration> getTargetConfigurations()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#compareTo(com.facebook.buck.core.model.targetgraph.MergedTargetNode)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(MergedTargetNode that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<MergedTargetNode>`
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
