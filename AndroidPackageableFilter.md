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
[Package]{.packageLabelInType} [com.facebook.buck.android.packageable](package-summary.html)
:::

## Interface AndroidPackageableFilter {#interface-androidpackageablefilter .title title="Interface AndroidPackageableFilter"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ConstraintBasedAndroidPackageableFilter`,
        `NoopAndroidPackageableFilter`

    ------------------------------------------------------------------------

        public interface AndroidPackageableFilter

    ::: block
    Encapsulates logic for filtering instances of
    [`AndroidPackageable`](AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
    when collecting targets from transitive dependencies of an Android
    binary.
    Targets are split in two categories: targets with native code (cxx
    libraries, etc.) and targets with non-native code (java libraries,
    Android resources).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `shouldExclud         | ::: block             |
        |                       | eNonNativeTarget​(Buil | Encapsulates the      |
        |                       | dTarget buildTarget)` | filtering logic of    |
        |                       |                       | non-native targets    |
        |                       |                       | (java libraries,      |
        |                       |                       | resources, etc.)      |
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

        []{#shouldExcludeNonNativeTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### shouldExcludeNonNativeTarget

            ``` methodSignature
            boolean shouldExcludeNonNativeTarget​(BuildTarget buildTarget)
            ```

            ::: block
            Encapsulates the filtering logic of non-native targets (java
            libraries, resources, etc.)
            :::

            [Returns:]{.returnLabel}
            :   `true` if the given target (that represents a target
                with non-native code, like java library or resources)
                should be excluded from the collection.
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
