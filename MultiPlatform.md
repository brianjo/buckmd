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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.platform](package-summary.html)
:::

## Interface MultiPlatform {#interface-multiplatform .title title="Interface MultiPlatform"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `NamedPlatform`, `Platform`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidMultiPlatform`

    ------------------------------------------------------------------------

        public interface MultiPlatform
        extends NamedPlatform

    ::: block
    A generic platform that encapsulates multiple other platforms. This
    is used to support building packages and binaries that support
    multiple platforms (for example, an Android binary).
    A multiplatform is a platform that has a base platform and multiple
    nested platforms. When this platform is used in the context that
    expects a single platform the base platform is used to match the
    constraints.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Platform`            | `getBasePlatform()`   | ::: block             |
        |                       |                       | Access base platform  |
        |                       |                       | of this platform, for |
        |                       |                       | example, CPU-neutral  |
        |                       |                       | Android platform      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `                     | ::: block             |
        | ollect.ImmutableColle | getNestedPlatforms()` | Access nested         |
        | ction<NamedPlatform>` |                       | platforms, for        |
        |                       |                       | example, per-CPU      |
        |                       |                       | platforms for Android |
        |                       |                       | platform              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `matchesAll​(Colle     |                       |
        |                       | ction<ConstraintValue |                       |
        |                       | > constraintValues,   |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.platform.NamedPlatform}

            ### Methods inherited from interface com.facebook.buck.core.model.platform.[NamedPlatform](NamedPlatform.html "interface in com.facebook.buck.core.model.platform")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#matchesAll(java.util.Collection,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### matchesAll

            ``` methodSignature
            default boolean matchesAll​(Collection<ConstraintValue> constraintValues,
                                       DependencyStack dependencyStack)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `matchesAll` in interface `Platform`

            [Returns:]{.returnLabel}
            :   `true` if the current platform matches the provided
                constraints.

        []{#getBasePlatform()}

        -   #### getBasePlatform

            ``` methodSignature
            Platform getBasePlatform()
            ```

            ::: block
            Access base platform of this platform, for example,
            CPU-neutral Android platform
            :::

        []{#getNestedPlatforms()}

        -   #### getNestedPlatforms

            ``` methodSignature
            com.google.common.collect.ImmutableCollection<NamedPlatform> getNestedPlatforms()
            ```

            ::: block
            Access nested platforms, for example, per-CPU platforms for
            Android platform
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
