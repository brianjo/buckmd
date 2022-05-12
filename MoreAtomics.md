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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class MoreAtomics {#class-moreatomics .title title="Class MoreAtomics"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.MoreAtomics

::: description
-   

    ------------------------------------------------------------------------

        public final class MoreAtomics
        extends Object

    ::: block
    Utility methods for common routines with atomic variables
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static long`         | `setMaxAndGet​(long v  | ::: block             |
        |                       | alue,             Ato | Update atomic         |
        |                       | micLong atomicValue)` | variable if provided  |
        |                       |                       | value is greater than |
        |                       |                       | value stored in       |
        |                       |                       | atomic variable.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static long`         | `setMinAndGet​(long v  | ::: block             |
        |                       | alue,             Ato | Update atomic         |
        |                       | micLong atomicValue)` | variable if provided  |
        |                       |                       | value is less than    |
        |                       |                       | value stored in       |
        |                       |                       | atomic variable.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setMaxAndGet(long,java.util.concurrent.atomic.AtomicLong)}

        -   #### setMaxAndGet

            ``` methodSignature
            public static long setMaxAndGet​(long value,
                                            AtomicLong atomicValue)
            ```

            ::: block
            Update atomic variable if provided value is greater than
            value stored in atomic variable. Implementation is
            lock-free.
            :::

            [Parameters:]{.paramLabel}
            :   `value` - A value to check against atomic value
            :   `atomicValue` - Atomic variable that will keep a maximum
                of two values

            [Returns:]{.returnLabel}
            :   New value of `atomicValue`

        []{#setMinAndGet(long,java.util.concurrent.atomic.AtomicLong)}

        -   #### setMinAndGet

            ``` methodSignature
            public static long setMinAndGet​(long value,
                                            AtomicLong atomicValue)
            ```

            ::: block
            Update atomic variable if provided value is less than value
            stored in atomic variable. Implementation is lock-free.
            :::

            [Parameters:]{.paramLabel}
            :   `value` - A value to check against atomic value
            :   `atomicValue` - Atomic variable that will keep a minimum
                of two values

            [Returns:]{.returnLabel}
            :   New value of `atomicValue`
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
