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
[Package]{.packageLabelInType} [com.facebook.buck.parser.exceptions](package-summary.html)
:::

## Class ParsingError {#class-parsingerror .title title="Class ParsingError"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.exceptions.ParsingError

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ParsingError
        extends Object

    ::: block
    Holds information about error occurred during parsing a build file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `ParsingError()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ParsingError` | `from​(Exception ex)`  | ::: block             |
        |                       |                       | Transform regular     |
        |                       |                       | Exception to parsing  |
        |                       |                       | error object          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getMessage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getStackTrace()`     |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ParsingError` | `of​(String message,   |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | <String> stackTrace)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### ParsingError

                public ParsingError()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            public abstract String getMessage()
            ```

            [Returns:]{.returnLabel}
            :   Human readable message of the error.

        []{#getStackTrace()}

        -   #### getStackTrace

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getStackTrace()
            ```

            [Returns:]{.returnLabel}
            :   Parser stack trace to the errorred callsite, if any.

        []{#from(java.lang.Exception)}

        -   #### from

            ``` methodSignature
            public static ParsingError from​(Exception ex)
            ```

            ::: block
            Transform regular Exception to parsing error object
            :::

        []{#of(java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static ParsingError of​(String message,
                                          com.google.common.collect.ImmutableList<String> stackTrace)
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
