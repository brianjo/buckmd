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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Interface RustToolchain {#interface-rusttoolchain .title title="Interface RustToolchain"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Toolchain`

    ------------------------------------------------------------------------

        public interface RustToolchain
        extends Toolchain

    ::: block
    Container for `RustPlatform`s.
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

          Modifier and Type                        Method                                                                                                   Description
          ---------------------------------------- -------------------------------------------------------------------------------------------------------- -------------
          `UnresolvedRustPlatform`                 `getDefaultRustPlatform()`                                                                                
          `default String`                         `getName()`                                                                                               
          `FlavorDomain<UnresolvedRustPlatform>`   `getRustPlatforms()`                                                                                      
          `static RustToolchain`                   `of​(UnresolvedRustPlatform defaultRustPlatform,   FlavorDomain<UnresolvedRustPlatform> rustPlatforms)`    

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
                Values](../../../../../constant-values.html#com.facebook.buck.features.rust.RustToolchain.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            default String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`

        []{#getDefaultRustPlatform()}

        -   #### getDefaultRustPlatform

            ``` methodSignature
            UnresolvedRustPlatform getDefaultRustPlatform()
            ```

        []{#getRustPlatforms()}

        -   #### getRustPlatforms

            ``` methodSignature
            FlavorDomain<UnresolvedRustPlatform> getRustPlatforms()
            ```

        []{#of(com.facebook.buck.features.rust.UnresolvedRustPlatform,com.facebook.buck.core.model.FlavorDomain)}

        -   #### of

            ``` methodSignature
            static RustToolchain of​(UnresolvedRustPlatform defaultRustPlatform,
                                    FlavorDomain<UnresolvedRustPlatform> rustPlatforms)
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
