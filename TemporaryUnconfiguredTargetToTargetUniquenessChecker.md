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
[Package]{.packageLabelInType} [com.facebook.buck.parser.temporarytargetuniquenesschecker](package-summary.html)
:::

## Interface TemporaryUnconfiguredTargetToTargetUniquenessChecker {#interface-temporaryunconfiguredtargettotargetuniquenesschecker .title title="Interface TemporaryUnconfiguredTargetToTargetUniquenessChecker"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface TemporaryUnconfiguredTargetToTargetUniquenessChecker

    ::: block
    Check there\'s only one
    [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
    for
    [`UnconfiguredBuildTarget`](../../core/model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model").
    We do that this until we use target configuration in the output
    path.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addTarget​(Buil       | ::: block             |
        |                       | dTarget buildTarget,  | Register a target,    |
        |                       |          DependencySt | check if there\'s     |
        |                       | ack dependencyStack)` | already registered    |
        |                       |                       | target with the same  |
        |                       |                       | unconfigured target,  |
        |                       |                       | same flavors but      |
        |                       |                       | different             |
        |                       |                       | configuration.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static TemporaryUn   | `creat                | ::: block             |
        | configuredTargetToTar | e​(boolean buckOutIncl | Create a uniqueness   |
        | getUniquenessChecker` | udeTargetConfigHash)` | checker, deny or      |
        |                       |                       | no-op depending on    |
        |                       |                       | hashed buck-out       |
        |                       |                       | disabled or enabled.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### addTarget

            ``` methodSignature
            void addTarget​(BuildTarget buildTarget,
                           DependencyStack dependencyStack)
            ```

            ::: block
            Register a target, check if there\'s already registered
            target with the same unconfigured target, same flavors but
            different configuration.
            :::

        []{#create(boolean)}

        -   #### create

            ``` methodSignature
            static TemporaryUnconfiguredTargetToTargetUniquenessChecker create​(boolean buckOutIncludeTargetConfigHash)
            ```

            ::: block
            Create a uniqueness checker, deny or no-op depending on
            hashed buck-out disabled or enabled.
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
