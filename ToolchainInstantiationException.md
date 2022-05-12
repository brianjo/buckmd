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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Class ToolchainInstantiationException {#class-toolchaininstantiationexception .title title="Class ToolchainInstantiationException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   [com.facebook.buck.core.exceptions.HumanReadableException](../exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

                -   -   com.facebook.buck.core.toolchain.ToolchainInstantiationException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ------------------------------------------------------------------------

        public class ToolchainInstantiationException
        extends HumanReadableException

    ::: block
    An exception that indicates a problem during toolchain creation.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.core.toolchain.ToolchainInstantiationException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ToolchainInstantiationException​(ExceptionWithHumanReadableMessage e)`                                                                                                
          `ToolchainInstantiationException​(String humanReadableErrorMessage)`                                                                                                   
          `ToolchainInstantiationException​(String humanReadableFormatString,                                Object... args)`                                                    
          `ToolchainInstantiationException​(Throwable cause,                                String humanReadableErrorMessage)`                                                   
          `ToolchainInstantiationException​(Throwable cause,                                String humanReadableFormatString,                                Object... args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                          Method                             Description
          ------------------------------------------ ---------------------------------- -------------
          `static ToolchainInstantiationException`   `wrap​(HumanReadableException e)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.HumanReadableException}

            ### Methods inherited from class com.facebook.buck.core.exceptions.[HumanReadableException](../exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

            `getDependencyStack, getHumanReadableErrorMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Throwable}

            ### Methods inherited from class java.lang.[Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.Object...)}

        -   #### ToolchainInstantiationException

                public ToolchainInstantiationException​(String humanReadableFormatString,
                                                       Object... args)

        []{#<init>(java.lang.String)}

        -   #### ToolchainInstantiationException

                public ToolchainInstantiationException​(String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,java.lang.String)}

        -   #### ToolchainInstantiationException

                public ToolchainInstantiationException​(@Nullable
                                                       Throwable cause,
                                                       String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### ToolchainInstantiationException

                public ToolchainInstantiationException​(@Nullable
                                                       Throwable cause,
                                                       String humanReadableFormatString,
                                                       Object... args)

        []{#<init>(com.facebook.buck.core.exceptions.ExceptionWithHumanReadableMessage)}

        -   #### ToolchainInstantiationException

                public ToolchainInstantiationException​(ExceptionWithHumanReadableMessage e)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#wrap(com.facebook.buck.core.exceptions.HumanReadableException)}

        -   #### wrap

            ``` methodSignature
            public static ToolchainInstantiationException wrap​(HumanReadableException e)
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
