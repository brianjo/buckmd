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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class CommandLineException {#class-commandlineexception .title title="Class CommandLineException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   [com.facebook.buck.core.exceptions.HumanReadableException](../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

                -   -   com.facebook.buck.util.CommandLineException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ------------------------------------------------------------------------

        public class CommandLineException
        extends HumanReadableException
        implements ExceptionWithHumanReadableMessage

    ::: block
    Exception that is raised when user-supplied command line contains
    incompatible parameters or in general cannot be executed
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../serialized-form.html#com.facebook.buck.util.CommandLineException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandLineException​(ExceptionWithHumanReadableMessage e)`                                                                          
          `CommandLineException​(String humanReadableErrorMessage)`                                                                             
          `CommandLineException​(String humanReadableFormatString,                     Object... args)`                                         
          `CommandLineException​(Throwable cause,                     String humanReadableErrorMessage)`                                        
          `CommandLineException​(Throwable cause,                     String humanReadableFormatString,                     Object... args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.HumanReadableException}

            ### Methods inherited from class com.facebook.buck.core.exceptions.[HumanReadableException](../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.ExceptionWithHumanReadableMessage}

            ### Methods inherited from interface com.facebook.buck.core.exceptions.[ExceptionWithHumanReadableMessage](../core/exceptions/ExceptionWithHumanReadableMessage.html "interface in com.facebook.buck.core.exceptions")

            `getDependencyStack, getHumanReadableErrorMessage`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.Object...)}

        -   #### CommandLineException

                public CommandLineException​(String humanReadableFormatString,
                                            Object... args)

        []{#<init>(java.lang.String)}

        -   #### CommandLineException

                public CommandLineException​(String humanReadableErrorMessage)

        []{#<init>(com.facebook.buck.core.exceptions.ExceptionWithHumanReadableMessage)}

        -   #### CommandLineException

                public CommandLineException​(ExceptionWithHumanReadableMessage e)

        []{#<init>(java.lang.Throwable,java.lang.String)}

        -   #### CommandLineException

                public CommandLineException​(@Nullable
                                            Throwable cause,
                                            String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### CommandLineException

                public CommandLineException​(@Nullable
                                            Throwable cause,
                                            String humanReadableFormatString,
                                            Object... args)
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
