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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ErrorLogger.DeconstructedException {#class-errorlogger.deconstructedexception .title title="Class ErrorLogger.DeconstructedException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ErrorLogger.DeconstructedException

::: description
-   

    Enclosing class:
    :   [ErrorLogger](ErrorLogger.html "class in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static class ErrorLogger.DeconstructedException
        extends Object

    ::: block
    The result of exception \"deconstruction\". Provides access to the
    user-friendly message with context.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getAugmentedErr      | ::: block             |
        |                       | orWithContext​(String  | Creates the           |
        |                       | indent,               | user-friendly         |
        |                       |                HumanR | exception with        |
        |                       | eadableExceptionAugme | context, masked stack |
        |                       | ntor errorAugmentor)` | trace (if not         |
        |                       |                       | suppressed), and with |
        |                       |                       | augmentations.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMessage​(boolean   | ::: block             |
        |                       | suppressStackTraces)` | Returns the message   |
        |                       |                       | (and optionally stack |
        |                       |                       | trace) for the root   |
        |                       |                       | cause.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Throwable`           | `getRootCause()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isNoSpaceOnDevice()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isUserError()`       | ::: block             |
        |                       |                       | Indicates whether     |
        |                       |                       | this exception is a   |
        |                       |                       | user error or a buck  |
        |                       |                       | internal error.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#getMessage(boolean)}

        -   #### getMessage

            ``` methodSignature
            public String getMessage​(boolean suppressStackTraces)
            ```

            ::: block
            Returns the message (and optionally stack trace) for the
            root cause.
            :::

        []{#isUserError()}

        -   #### isUserError

            ``` methodSignature
            public boolean isUserError()
            ```

            ::: block
            Indicates whether this exception is a user error or a buck
            internal error.
            :::

        []{#isNoSpaceOnDevice()}

        -   #### isNoSpaceOnDevice

            ``` methodSignature
            public boolean isNoSpaceOnDevice()
            ```

        []{#getRootCause()}

        -   #### getRootCause

            ``` methodSignature
            public Throwable getRootCause()
            ```

        []{#getAugmentedErrorWithContext(java.lang.String,com.facebook.buck.core.exceptions.HumanReadableExceptionAugmentor)}

        -   #### getAugmentedErrorWithContext

            ``` methodSignature
            public String getAugmentedErrorWithContext​(String indent,
                                                       HumanReadableExceptionAugmentor errorAugmentor)
            ```

            ::: block
            Creates the user-friendly exception with context, masked
            stack trace (if not suppressed), and with augmentations.
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
