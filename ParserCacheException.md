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
[Package]{.packageLabelInType} [com.facebook.buck.parser.cache](package-summary.html)
:::

## Class ParserCacheException {#class-parsercacheexception .title title="Class ParserCacheException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   com.facebook.buck.parser.cache.ParserCacheException

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`

    ------------------------------------------------------------------------

        public class ParserCacheException
        extends Exception

    ::: block
    This exception is thrown when there are failures while doing
    `ParserCacheStorage` operations.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.parser.cache.ParserCacheException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Pars                             | ::: block                         |
        | erCacheException​(String message)` | Constructs a                      |
        |                                   | `ParserCacheException` object     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ParserCacheE                     | ::: block                         |
        | xception​(String format,           | Constructs a                      |
        |            Object... parameters)` | `ParserCacheException` object     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ParserCa                         | ::: block                         |
        | cheException​(Throwable cause,     | Constructs a                      |
        |                  String message)` | `ParserCacheException` object     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ParserCacheExcep                 | ::: block                         |
        | tion​(Throwable cause,             | Constructs a                      |
        |          String format,           | `ParserCacheException` object     |
        |            Object... parameters)` | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

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

        []{#<init>(java.lang.String)}

        -   #### ParserCacheException

                public ParserCacheException​(String message)

            ::: block
            Constructs a `ParserCacheException` object
            :::

            [Parameters:]{.paramLabel}
            :   `message` - the message of the Exception.

        []{#<init>(java.lang.Throwable,java.lang.String)}

        -   #### ParserCacheException

                public ParserCacheException​(Throwable cause,
                                            String message)

            ::: block
            Constructs a `ParserCacheException` object
            :::

            [Parameters:]{.paramLabel}
            :   `cause` - the cause for this exception
            :   `message` - the message of the Exception.

        []{#<init>(java.lang.String,java.lang.Object...)}

        -   #### ParserCacheException

                public ParserCacheException​(String format,
                                            Object... parameters)

            ::: block
            Constructs a `ParserCacheException` object
            :::

            [Parameters:]{.paramLabel}
            :   `format` - a format
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}
                to create the
                [`ParserCacheException`](ParserCacheException.html "class in com.facebook.buck.parser.cache")
                message.
            :   `parameters` - the parameters for formatting the
                message.

        []{#<init>(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### ParserCacheException

                public ParserCacheException​(Throwable cause,
                                            String format,
                                            Object... parameters)

            ::: block
            Constructs a `ParserCacheException` object
            :::

            [Parameters:]{.paramLabel}
            :   `cause` - the cause for this exception
            :   `format` - a format
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}
                to create the
                [`ParserCacheException`](ParserCacheException.html "class in com.facebook.buck.parser.cache")
                message.
            :   `parameters` - the parameters for formatting the
                message.
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
