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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class ConfigurationBuildTargets {#class-configurationbuildtargets .title title="Class ConfigurationBuildTargets"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.ConfigurationBuildTargets

::: description
-   

    ------------------------------------------------------------------------

        public class ConfigurationBuildTargets
        extends Object

    ::: block
    Encapsulates logic to convert
    [`UnconfiguredBuildTarget`](UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
    that represents a configuration target to an instance of
    [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model").
    We represent configuration targets as
    [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model")
    (targets with a configuration) as oppose to
    [`UnconfiguredBuildTarget`](UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
    to keep target graph model consistent and in one place
    ([`TargetGraph`](targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    uses
    [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model")
    only). This also allows us to avoid adding special handling for
    unconfigured targets in many other places (for example, in places
    with generic graph analysis like in `query` command).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static BuildTarget`  | `con                  |                       |
        |                       | vert​(UnconfiguredBuil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `co                   | ::: block             |
        | .common.collect.Immut | nvert​(com.google.comm | Performs conversion   |
        | ableSet<BuildTarget>` | on.collect.ImmutableS | similar to            |
        |                       | et<UnconfiguredBuildT | [`convert(Unconf      |
        |                       | arget> buildTargets)` | iguredBuildTarget)`]( |
        |                       |                       | #convert(com.facebook |
        |                       |                       | .buck.core.model.Unco |
        |                       |                       | nfiguredBuildTarget)) |
        |                       |                       | for a set of targets. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static O             | `convert​(Optio        | ::: block             |
        | ptional<BuildTarget>` | nal<UnconfiguredBuild | Performs conversion   |
        |                       | Target> buildTarget)` | similar to            |
        |                       |                       | [`convert(Unconf      |
        |                       |                       | iguredBuildTarget)`]( |
        |                       |                       | #convert(com.facebook |
        |                       |                       | .buck.core.model.Unco |
        |                       |                       | nfiguredBuildTarget)) |
        |                       |                       | for an optional       |
        |                       |                       | value.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `c                    | ::: block             |
        | atic <T> com.google.c | onvertValues​(com.goog | Applies conversion    |
        | ommon.collect.Immutab | le.common.collect.Imm | similar to            |
        | leMap<T,​BuildTarget>` | utableMap<T,​Unconfigu | [`convert(Unconf      |
        |                       | redBuildTarget> map)` | iguredBuildTarget)`]( |
        |                       |                       | #convert(com.facebook |
        |                       |                       | .buck.core.model.Unco |
        |                       |                       | nfiguredBuildTarget)) |
        |                       |                       | to values in a map.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <             | `convert              | ::: block             |
        | T extends Comparable< | Values​(com.google.com | Applies conversion    |
        | T>>com.google.common. | mon.collect.Immutable | similar to            |
        | collect.ImmutableSort | SortedMap<T,​Unconfigu | [`convert(Unconf      |
        | edMap<T,​BuildTarget>` | redBuildTarget> map)` | iguredBuildTarget)`]( |
        |                       |                       | #convert(com.facebook |
        |                       |                       | .buck.core.model.Unco |
        |                       |                       | nfiguredBuildTarget)) |
        |                       |                       | to values in a map.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#convert(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### convert

            ``` methodSignature
            public static BuildTarget convert​(UnconfiguredBuildTarget buildTarget)
            ```

            [Returns:]{.returnLabel}
            :   [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model")
                that corresponds to a given
                [`UnconfiguredBuildTarget`](UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model").

        []{#convert(java.util.Optional)}

        -   #### convert

            ``` methodSignature
            public static Optional<BuildTarget> convert​(Optional<UnconfiguredBuildTarget> buildTarget)
            ```

            ::: block
            Performs conversion similar to
            [`convert(UnconfiguredBuildTarget)`](#convert(com.facebook.buck.core.model.UnconfiguredBuildTarget))
            for an optional value.
            :::

        []{#convert(com.google.common.collect.ImmutableSet)}

        -   #### convert

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<BuildTarget> convert​(com.google.common.collect.ImmutableSet<UnconfiguredBuildTarget> buildTargets)
            ```

            ::: block
            Performs conversion similar to
            [`convert(UnconfiguredBuildTarget)`](#convert(com.facebook.buck.core.model.UnconfiguredBuildTarget))
            for a set of targets.
            :::

        []{#convertValues(com.google.common.collect.ImmutableMap)}

        -   #### convertValues

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableMap<T,​BuildTarget> convertValues​(com.google.common.collect.ImmutableMap<T,​UnconfiguredBuildTarget> map)
            ```

            ::: block
            Applies conversion similar to
            [`convert(UnconfiguredBuildTarget)`](#convert(com.facebook.buck.core.model.UnconfiguredBuildTarget))
            to values in a map.
            :::

        []{#convertValues(com.google.common.collect.ImmutableSortedMap)}

        -   #### convertValues

            ``` methodSignature
            public static <T extends Comparable<T>> com.google.common.collect.ImmutableSortedMap<T,​BuildTarget> convertValues​(com.google.common.collect.ImmutableSortedMap<T,​UnconfiguredBuildTarget> map)
            ```

            ::: block
            Applies conversion similar to
            [`convert(UnconfiguredBuildTarget)`](#convert(com.facebook.buck.core.model.UnconfiguredBuildTarget))
            to values in a map.
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
