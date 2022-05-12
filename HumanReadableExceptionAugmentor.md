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
[Package]{.packageLabelInType} [com.facebook.buck.core.exceptions](package-summary.html)
:::

## Class HumanReadableExceptionAugmentor {#class-humanreadableexceptionaugmentor .title title="Class HumanReadableExceptionAugmentor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.exceptions.HumanReadableExceptionAugmentor

::: description
-   

    ------------------------------------------------------------------------

        public class HumanReadableExceptionAugmentor
        extends Object

    ::: block
    A class that can append additional information to a
    HumanReadableException based on configuration settings. This can be
    useful, e.g., when there\'s a common parse error whose cause is not
    immediately visible.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `H                                | ::: block                         |
        | umanReadableExceptionAugmentor​(Ma | Create an instance of             |
        | p<Pattern,​String> augmentations)` | [`HumanReadableExce               |
        |                                   | ptionAugmentor`](HumanReadableExc |
        |                                   | eptionAugmentor.html "class in co |
        |                                   | m.facebook.buck.core.exceptions") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getAugment           | ::: block             |
        |                       | edError​(String humanR | Adds messages to the  |
        |                       | eadableErrorMessage)` | end of an existing    |
        |                       |                       | error message based   |
        |                       |                       | on regular            |
        |                       |                       | expressions provided  |
        |                       |                       | in .buckconfig.       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Map)}

        -   #### HumanReadableExceptionAugmentor

                public HumanReadableExceptionAugmentor​(Map<Pattern,​String> augmentations)

            ::: block
            Create an instance of
            [`HumanReadableExceptionAugmentor`](HumanReadableExceptionAugmentor.html "class in com.facebook.buck.core.exceptions")
            :::

            [Parameters:]{.paramLabel}
            :   `augmentations` - A mapping of regexes to the
                replacement strings to append to the end of error
                messages
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAugmentedError(java.lang.String)}

        -   #### getAugmentedError

            ``` methodSignature
            public String getAugmentedError​(String humanReadableErrorMessage)
            ```

            ::: block
            Adds messages to the end of an existing error message based
            on regular expressions provided in .buckconfig.
            If replacement fails (due to a configuration error, such as
            invalid regex), then a warning will be added to the returned
            message
            :::

            [Returns:]{.returnLabel}
            :   The original error message, with any error augmentations
                that this message matches appended to the end
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
