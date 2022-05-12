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
[Package]{.packageLabelInType} [com.facebook.buck.util.function](package-summary.html)
:::

## Interface TriFunction\<T,​U,​V,​R\> {#interface-trifunctiontuvr .title title="Interface TriFunction"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the type of the first argument to the function
    :   `U` - the type of the second argument to the function
    :   `V` - the type of the third argument to the function
    :   `R` - the type of the result of the function

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface TriFunction<T,​U,​V,​R>

    ::: block
    Represents a function that accepts four arguments and produces a
    result. This is the four-arity specialization of `Function`.
    This is a functional interface whose functional method is
    [`apply(Object, Object, Object  )`](#apply(T,U,V)).
    :::

    [See Also:]{.seeLabel}
    :   `Function`
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `R`                   | `apply​(T t,           | ::: block             |
        |                       |       U u,      V v)` | Applies this function |
        |                       |                       | to the given          |
        |                       |                       | arguments.            |
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

        []{#apply(java.lang.Object,java.lang.Object,java.lang.Object)}
        []{#apply(T,U,V)}

        -   #### apply

            ``` methodSignature
            R apply​(T t,
                    U u,
                    V v)
            ```

            ::: block
            Applies this function to the given arguments.
            :::

            [Parameters:]{.paramLabel}
            :   `t` - the first function argument
            :   `u` - the second function argument
            :   `v` - the third function argument

            [Returns:]{.returnLabel}
            :   the function result
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
