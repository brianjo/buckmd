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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Interface HasDesugarSupport {#interface-hasdesugarsupport .title title="Interface HasDesugarSupport"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `JavaLibrary`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `DefaultJavaLibrary`,
        `PrebuiltJar`

    ------------------------------------------------------------------------

        public interface HasDesugarSupport

    ::: block
    Implemented by build rules that support desugar process to the lower
    java versions, for example java 8 to java 7 desugar for Android
    builds.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `isDesugarEnabled()`  | ::: block             |
        |                       |                       | Desugar support for   |
        |                       |                       | java 8 features       |
        |                       |                       | withing single class  |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isInterfaceMet       | ::: block             |
        |                       | hodsDesugarEnabled()` | Desugar support for   |
        |                       |                       | interface default and |
        |                       |                       | static methods.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isDesugarEnabled()}

        -   #### isDesugarEnabled

            ``` methodSignature
            default boolean isDesugarEnabled()
            ```

            ::: block
            Desugar support for java 8 features withing single class
            file.
            Such as Lambda expressions, Method references, Repeating
            annotations
            :::

        []{#isInterfaceMethodsDesugarEnabled()}

        -   #### isInterfaceMethodsDesugarEnabled

            ``` methodSignature
            default boolean isInterfaceMethodsDesugarEnabled()
            ```

            ::: block
            Desugar support for interface default and static methods.
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
