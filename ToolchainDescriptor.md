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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Interface ToolchainDescriptor\<T extends [Toolchain](Toolchain.html "interface in com.facebook.buck.core.toolchain")\> {#interface-toolchaindescriptort-extends-toolchain .title title="Interface ToolchainDescriptor"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ToolchainDescriptor<T extends Toolchain>

    ::: block
    Contains basic information about a
    [`Toolchain`](Toolchain.html "interface in com.facebook.buck.core.toolchain")
    that can be used to identify and construct an instance of a
    particular Toolchain.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                      Method                                                                                                       Description
          ------------------------------------------------------ ------------------------------------------------------------------------------------------------------------ -------------
          `String`                                               `getName()`                                                                                                   
          `Class<T>`                                             `getToolchainClass()`                                                                                         
          `Class<? extends ToolchainFactory<T>>`                 `getToolchainFactoryClass()`                                                                                  
          `static <T extends Toolchain>ToolchainDescriptor<T>`   `of​(String name,   Class<T> toolchainClass,   Class<? extends ToolchainFactory<T>> toolchainFactoryClass)`    

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

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

        []{#getToolchainClass()}

        -   #### getToolchainClass

            ``` methodSignature
            Class<T> getToolchainClass()
            ```

        []{#getToolchainFactoryClass()}

        -   #### getToolchainFactoryClass

            ``` methodSignature
            Class<? extends ToolchainFactory<T>> getToolchainFactoryClass()
            ```

        []{#of(java.lang.String,java.lang.Class,java.lang.Class)}

        -   #### of

            ``` methodSignature
            static <T extends Toolchain> ToolchainDescriptor<T> of​(String name,
                                                                   Class<T> toolchainClass,
                                                                   Class<? extends ToolchainFactory<T>> toolchainFactoryClass)
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
