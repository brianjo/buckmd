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

## Interface ThrowingFunction\<T,​R,​E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#interface-throwingfunctiontre-extends-exception .title title="Interface ThrowingFunction"}
:::

::: contentContainer
::: description
-   

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface ThrowingFunction<T,​R,​E extends Exception>

    ::: block
    This version of `Function<T, R>` that can throw an exception.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `R`                   | `apply​(T t)`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default java.util.fu | `asFunction()`        | ::: block             |
        | nction.Function<T,​R>` |                       | Returns a Function    |
        |                       |                       | that will wrap any    |
        |                       |                       | thrown exception in a |
        |                       |                       | RuntimeException.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `asFunction​(Thr       | ::: block             |
        | <T2,​R2,​E2 extends Exc | owingFunction<T2,​R2,​E | A simple helper for   |
        | eption>java.util.func | 2> throwingFunction)` | constructing a        |
        | tion.Function<T2,​R2>` |                       | Function from a       |
        |                       |                       | throwing lambda.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#apply(java.lang.Object)} []{#apply(T)}

        -   #### apply

            ``` methodSignature
            R apply​(T t)
             throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#asFunction()}

        -   #### asFunction

            ``` methodSignature
            default java.util.function.Function<T,​R> asFunction()
            ```

            ::: block
            Returns a Function that will wrap any thrown exception in a
            RuntimeException.
            :::

        []{#asFunction(com.facebook.buck.util.function.ThrowingFunction)}

        -   #### asFunction

            ``` methodSignature
            static <T2,​R2,​E2 extends Exception> java.util.function.Function<T2,​R2> asFunction​(ThrowingFunction<T2,​R2,​E2> throwingFunction)
            ```

            ::: block
            A simple helper for constructing a Function from a throwing
            lambda.
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
