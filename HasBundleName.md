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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Interface HasBundleName {#interface-hasbundlename .title title="Interface HasBundleName"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `JsBundleDescriptionArg`, `JsBundleGenruleDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasBundleName

    ::: block
    Common interface for rule args that have a bundle name that can
    optionally be overridden depending on the flavors a rule is built
    with.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default String`      | `computeBundleName​(co | ::: block             |
        |                       | m.google.common.colle | Computes the bundle   |
        |                       | ct.ImmutableSortedSet | name as configured,   |
        |                       | <Flavor> flavors,     | or falls back to a    |
        |                       |               java.ut | default name.         |
        |                       | il.function.Supplier< | :::                   |
        |                       | String> defaultName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getBundleName()`     | ::: block             |
        |                       |                       | The name of the       |
        |                       |                       | bundle.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `getB                 | ::: block             |
        | ollect.ImmutableList< | undleNameForFlavor()` | A mapping from        |
        | Pair<Flavor,​String>>` |                       | flavors to bundle     |
        |                       |                       | names.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#computeBundleName(com.google.common.collect.ImmutableSortedSet,java.util.function.Supplier)}

        -   #### computeBundleName

            ``` methodSignature
            default String computeBundleName​(com.google.common.collect.ImmutableSortedSet<Flavor> flavors,
                                             java.util.function.Supplier<String> defaultName)
            ```

            ::: block
            Computes the bundle name as configured, or falls back to a
            default name.
            :::

        []{#getBundleName()}

        -   #### getBundleName

            ``` methodSignature
            Optional<String> getBundleName()
            ```

            ::: block
            The name of the bundle.
            :::

        []{#getBundleNameForFlavor()}

        -   #### getBundleNameForFlavor

            ``` methodSignature
            com.google.common.collect.ImmutableList<Pair<Flavor,​String>> getBundleNameForFlavor()
            ```

            ::: block
            A mapping from flavors to bundle names.
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
