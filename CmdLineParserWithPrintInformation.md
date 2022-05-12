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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.args](package-summary.html)
:::

## Class CmdLineParserWithPrintInformation {#class-cmdlineparserwithprintinformation .title title="Class CmdLineParserWithPrintInformation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.CmdLineParser

    -   -   com.facebook.buck.support.cli.args.CmdLineParserWithPrintInformation

::: description
-   

    ------------------------------------------------------------------------

        public class CmdLineParserWithPrintInformation
        extends org.kohsuke.args4j.CmdLineParser

    ::: block
    An implementation of `CmdLineParser` that can provide some
    information that can be used to print help in more flexible form
    than `CmdLineParser`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                        Description
          -------------------------------------------------- -------------
          `CmdLineParserWithPrintInformation​(Object bean)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `calculateMaxLen()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printUsage​(Writ      | ::: block             |
        |                       | er out,           org | Prints usage using    |
        |                       | .kohsuke.args4j.Optio | the provided length   |
        |                       | nHandlerFilter filter | to print options      |
        |                       | ,           int len)` | (instead of           |
        |                       |                       | calculating the       |
        |                       |                       | length as in          |
        |                       |                       | `CmdLineParser`).     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.kohsuke.args4j.CmdLineParser}

            ### Methods inherited from class org.kohsuke.args4j.CmdLineParser

            `addArgument, addOption, createOptionHandler, getArguments, getOptions, getProperties, isOption, parseArgument, parseArgument, printExample, printExample, printExample, printExample, printOption, printSingleLineUsage, printSingleLineUsage, printUsage, printUsage, printUsage, registerHandler, setUsageWidth, stopOptionParsing`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.Object)}

        -   #### CmdLineParserWithPrintInformation

                public CmdLineParserWithPrintInformation​(Object bean)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#calculateMaxLen()}

        -   #### calculateMaxLen

            ``` methodSignature
            public int calculateMaxLen()
            ```

            [Returns:]{.returnLabel}
            :   the maximum length of the options and arguments.

        []{#printUsage(java.io.Writer,org.kohsuke.args4j.OptionHandlerFilter,int)}

        -   #### printUsage

            ``` methodSignature
            public void printUsage​(Writer out,
                                   org.kohsuke.args4j.OptionHandlerFilter filter,
                                   int len)
            ```

            ::: block
            Prints usage using the provided length to print options
            (instead of calculating the length as in `CmdLineParser`).
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
