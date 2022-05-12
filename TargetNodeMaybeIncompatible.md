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

## Class TargetNodeMaybeIncompatible {#class-targetnodemaybeincompatible .title title="Class TargetNodeMaybeIncompatible"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.TargetNodeMaybeIncompatible

::: description
-   

    ------------------------------------------------------------------------

        public class TargetNodeMaybeIncompatible
        extends Object

    ::: block
    This may have a TargetNode or some diagnostic information, in case
    the target was found incompatible.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `TargetNode<?>`       | `assertGetTa          |                       |
        |                       | rgetNode​(DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableList<Unco |                       |                       |
        | nfiguredBuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `get                  |                       |
        | ional<TargetNode<?>>` | TargetNodeOptional()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static TargetN       | `ofCompatible​(Targe   | ::: block             |
        | odeMaybeIncompatible` | tNode<?> targetNode)` | Constructor to create |
        |                       |                       | object for a          |
        |                       |                       | compatible target     |
        |                       |                       | node.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static TargetN       | `ofIn                 | ::: block             |
        | odeMaybeIncompatible` | compatible​(BuildTarge | Constructor to create |
        |                       | t target,             | object for a target   |
        |                       |    com.google.common. | node which was        |
        |                       | collect.ImmutableList | incompatible.         |
        |                       | <UnconfiguredBuildTar | :::                   |
        |                       | get> compatibleWith)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ofIncompatible(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList)}

        -   #### ofIncompatible

            ``` methodSignature
            public static TargetNodeMaybeIncompatible ofIncompatible​(BuildTarget target,
                                                                     com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> compatibleWith)
            ```

            ::: block
            Constructor to create object for a target node which was
            incompatible.
            :::

        []{#ofCompatible(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### ofCompatible

            ``` methodSignature
            public static TargetNodeMaybeIncompatible ofCompatible​(TargetNode<?> targetNode)
            ```

            ::: block
            Constructor to create object for a compatible target node.
            :::

        []{#assertGetTargetNode(com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### assertGetTargetNode

            ``` methodSignature
            public TargetNode<?> assertGetTargetNode​(DependencyStack dependencyStack)
            ```

        []{#getTargetNodeOptional()}

        -   #### getTargetNodeOptional

            ``` methodSignature
            public Optional<TargetNode<?>> getTargetNodeOptional()
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
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
