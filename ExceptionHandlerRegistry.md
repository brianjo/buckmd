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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class ExceptionHandlerRegistry\<R\> {#class-exceptionhandlerregistryr .title title="Class ExceptionHandlerRegistry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.exceptions.handler.ExceptionHandlerRegistry\<R\>

::: description
-   

    ------------------------------------------------------------------------

        public class ExceptionHandlerRegistry<R>
        extends Object

    ::: block
    Central registry to manage different kinds of exceptions thrown to
    Buck Main class level, which will unwrap the exceptions when
    necessary to make exceptions more friendly and readable to users
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ExceptionHandlerRegistry​(com.google.common.collect.ImmutableList<ExceptionHandler<? extends Throwable,​R>> handlers,                         ExceptionHandler<Throwable,​R> genericHandler)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                           Description
          ------------------- -------------------------------- -------------
          `R`                 `handleException​(Throwable t)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableList,com.facebook.buck.support.exceptions.handler.ExceptionHandler)}

        -   #### ExceptionHandlerRegistry

                public ExceptionHandlerRegistry​(com.google.common.collect.ImmutableList<ExceptionHandler<? extends Throwable,​R>> handlers,
                                                ExceptionHandler<Throwable,​R> genericHandler)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#handleException(java.lang.Throwable)}

        -   #### handleException

            ``` methodSignature
            public R handleException​(Throwable t)
            ```

            [Parameters:]{.paramLabel}
            :   `t` - the exception to handle

            [Returns:]{.returnLabel}

            :   the exit code Buck should return to user

                This method tries to find a registered
                [`ExceptionHandler`](ExceptionHandler.html "class in com.facebook.buck.support.exceptions.handler")
                that can process the input Exception, and calls that
                handler to process the exception. If it cannot find one,
                it will try to unwrap the exception by calling
                getCause() to get underlying exceptions. If all the
                underlying causes are exhausted, or any loop is detected
                in the exception chain before an exception is handled,
                the top level Throwable will be processed by the
                genericHandler.
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
