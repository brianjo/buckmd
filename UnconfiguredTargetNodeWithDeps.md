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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class UnconfiguredTargetNodeWithDeps {#class-unconfiguredtargetnodewithdeps .title title="Class UnconfiguredTargetNodeWithDeps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.raw.UnconfiguredTargetNodeWithDeps

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`

    ------------------------------------------------------------------------

        public abstract class UnconfiguredTargetNodeWithDeps
        extends Object
        implements ComputeResult

    ::: block
    A pair of
    [`UnconfiguredTargetNode`](UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
    and its dependencies
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `UnconfiguredT        | ::: block             |
        |                       | argetNodeWithDeps.Unc | This mixin is used by |
        |                       | onfiguredTargetNodeWi | JSON serializer to    |
        |                       | thDepsUnwrappedMixin` | flatten               |
        |                       |                       | [`Unconfig            |
        |                       |                       | uredTargetNode`](Unco |
        |                       |                       | nfiguredTargetNode.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.mo |
        |                       |                       | del.targetgraph.raw") |
        |                       |                       | properties We cannot  |
        |                       |                       | use `JsonUnwrapped`   |
        |                       |                       | directly on           |
        |                       |                       | [`getUnconfiguredTa   |
        |                       |                       | rgetNode()`](#getUnco |
        |                       |                       | nfiguredTargetNode()) |
        |                       |                       | because it is not     |
        |                       |                       | supported by typed    |
        |                       |                       | deserializer          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                          Description
          ------------------------------------ -------------
          `UnconfiguredTargetNodeWithDeps()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract c           | `getDeps()`           | ::: block             |
        | om.google.common.coll |                       | List of build targets |
        | ect.ImmutableSet<Unco |                       | that this node        |
        | nfiguredBuildTarget>` |                       | depends on.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Un          | `getUnco              | ::: block             |
        | configuredTargetNode` | nfiguredTargetNode()` | Raw target node, i.e. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Unconfigur    | `of​(UnconfiguredTa    |                       |
        | edTargetNodeWithDeps` | rgetNode unconfigured |                       |
        |                       | TargetNode,   com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableSet<Unconfigur |                       |
        |                       | edBuildTarget> deps)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### UnconfiguredTargetNodeWithDeps

                public UnconfiguredTargetNodeWithDeps()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnconfiguredTargetNode()}

        -   #### getUnconfiguredTargetNode

            ``` methodSignature
            public abstract UnconfiguredTargetNode getUnconfiguredTargetNode()
            ```

            ::: block
            Raw target node, i.e. a target node with partially resolved
            attributes
            :::

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<UnconfiguredBuildTarget> getDeps()
            ```

            ::: block
            List of build targets that this node depends on. Because
            [`UnconfiguredTargetNode`](UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            may have unresolved configuration, this list is excessive,
            i.e. may contain all possible dependents for all possible
            configurations.
            :::

        []{#of(com.facebook.buck.core.model.targetgraph.raw.UnconfiguredTargetNode,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredTargetNodeWithDeps of​(UnconfiguredTargetNode unconfiguredTargetNode,
                                                            com.google.common.collect.ImmutableSet<UnconfiguredBuildTarget> deps)
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
