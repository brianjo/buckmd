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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain](package-summary.html)
:::

## Interface AdbToolchain {#interface-adbtoolchain .title title="Interface AdbToolchain"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Toolchain`

    ------------------------------------------------------------------------

        public interface AdbToolchain
        extends Toolchain

    ::: block
    The adb Android tool.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field            Description
          ------------------- ---------------- -------------
          `static String`     `DEFAULT_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method               Description
          ----------------------- -------------------- -------------
          `Path`                  `getAdbPath()`        
          `default String`        `getName()`           
          `static AdbToolchain`   `of​(Path adbPath)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_NAME}

        -   #### DEFAULT_NAME

                static final String DEFAULT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.toolchain.AdbToolchain.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            static AdbToolchain of​(Path adbPath)
            ```

        []{#getAdbPath()}

        -   #### getAdbPath

            ``` methodSignature
            Path getAdbPath()
            ```

            [Returns:]{.returnLabel}
            :   `Path` pointing to the Android adb platform tool.

        []{#getName()}

        -   #### getName

            ``` methodSignature
            default String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::