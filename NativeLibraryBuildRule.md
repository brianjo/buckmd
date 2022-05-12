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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface NativeLibraryBuildRule {#interface-nativelibrarybuildrule .title title="Interface NativeLibraryBuildRule"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `NdkLibrary`, `PrebuiltNativeLibrary`

    ------------------------------------------------------------------------

        public interface NativeLibraryBuildRule

    ::: block
    [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    that contains various `.so` files for Android, organized by target
    CPU architecture.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getLibraryPath()`    | ::: block             |
        |                       |                       | Returns the path to   |
        |                       |                       | the directory         |
        |                       |                       | containing `.so`      |
        |                       |                       | files organized by    |
        |                       |                       | target CPU            |
        |                       |                       | architecture.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAsset()`           |                       |
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

        []{#isAsset()}

        -   #### isAsset

            ``` methodSignature
            boolean isAsset()
            ```

            [Returns:]{.returnLabel}
            :   A boolean indicating whether the `.so` files in the
                directory returned by
                [`getLibraryPath()`](#getLibraryPath()) should be
                included in the `assets` folder in the APK.

        []{#getLibraryPath()}

        -   #### getLibraryPath

            ``` methodSignature
            Path getLibraryPath()
            ```

            ::: block
            Returns the path to the directory containing `.so` files
            organized by target CPU architecture. This often contains
            subdirectories such as:
            -   `armeabi`
            -   `armeabi-v7a`
            :::

            [Returns:]{.returnLabel}
            :   A path relative to the project root that should does
                *not* include a trailing slash.
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
