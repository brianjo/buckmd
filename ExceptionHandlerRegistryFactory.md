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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.support.exceptions.handler](package-summary.html)
:::

## Class ExceptionHandlerRegistryFactory {#class-exceptionhandlerregistryfactory .title title="Class ExceptionHandlerRegistryFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.exceptions.handler.ExceptionHandlerRegistryFactory

::: description
-   

    ------------------------------------------------------------------------

        public class ExceptionHandlerRegistryFactory
        extends Object

    ::: block
    Util class for creating an
    [`ExceptionHandlerRegistry`](ExceptionHandlerRegistry.html "class in com.facebook.buck.support.exceptions.handler")
    with the default defaultHandlers
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `create()`            |                       |
        | static ExceptionHandl |                       |                       |
        | erRegistry<ExitCode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `create​(Except        | ::: block             |
        | static ExceptionHandl | ionHandler<? extends  | Overriding is defined |
        | erRegistry<ExitCode>` | Throwable,​ExitCode>.. | such that the order   |
        |                       | . exceptionHandlers)` | of the existing       |
        |                       |                       | handlers are          |
        |                       |                       | unaltered.            |
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

        []{#create(com.facebook.buck.support.exceptions.handler.ExceptionHandler...)}

        -   #### create

            ``` methodSignature
            @SafeVarargs
            public static ExceptionHandlerRegistry<ExitCode> create​(ExceptionHandler<? extends Throwable,​ExitCode>... exceptionHandlers)
            ```

            ::: block
            Overriding is defined such that the order of the existing
            handlers are unaltered. When handlers handle the same
            exception, the new one will replace the existing handler.
            New handlers not present in the mapping will be appended at
            the end of the handling chain.
            :::

            [Parameters:]{.paramLabel}
            :   `exceptionHandlers` - the defaultHandlers to override
                some default handler

            [Returns:]{.returnLabel}
            :   new
                [`ExceptionHandlerRegistry`](ExceptionHandlerRegistry.html "class in com.facebook.buck.support.exceptions.handler")
                with the default defaultHandlers overridden by the given
                ones

        []{#create()}

        -   #### create

            ``` methodSignature
            public static ExceptionHandlerRegistry<ExitCode> create()
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`ExceptionHandlerRegistry`](ExceptionHandlerRegistry.html "class in com.facebook.buck.support.exceptions.handler")
                with the default handlers
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
