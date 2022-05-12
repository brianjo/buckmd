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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class CommandHelper {#class-commandhelper .title title="Class CommandHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.CommandHelper

::: description
-   

    ------------------------------------------------------------------------

        public final class CommandHelper
        extends Object

    ::: block
    Utility class with print methods
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `maybePrintShowO      | ::: block             |
        |                       | utputWarning​(CliConfi | Prints a warning to   |
        |                       | g cliConfig,          | terminal about        |
        |                       |                    An | \--show-output being  |
        |                       | si ansi,              | replaced by           |
        |                       |                BuckEv | \--show-outputs if    |
        |                       | entBus buckEventBus)` | the warning is        |
        |                       |                       | enabled in the buck   |
        |                       |                       | config and the        |
        |                       |                       | environment supports  |
        |                       |                       | ANSI.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `print​(com.           | ::: block             |
        |                       | google.common.collect | Prints target and     |
        |                       | .Multimap<String,​Quer | dependencies map into |
        |                       | yTarget> targetsAndDe | printStream.          |
        |                       | pendencies,      Prin | :::                   |
        |                       | tStream printStream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `print​(Set<QueryTarge | ::: block             |
        |                       | t> targets,      Prin | Prints target set     |
        |                       | tStream printStream)` | into printStream.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `prin                 | ::: block             |
        |                       | tJsonOutput​(com.googl | Prints target and     |
        |                       | e.common.collect.Mult | result map\'s json    |
        |                       | imap<String,​QueryTarg | representation into   |
        |                       | et> targetsAndResults | printStream.          |
        |                       | ,                Prin | :::                   |
        |                       | tStream printStream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `printJsonOutput​(Set  | ::: block             |
        |                       | <QueryTarget> targets | Prints targets set    |
        |                       | ,                Prin | json representation   |
        |                       | tStream printStream)` | into printStream.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `p                    | ::: block             |
        |                       | rintShortDescription​( | Prints short          |
        |                       | Command command,      | description of a      |
        |                       |                  Prin | given command into    |
        |                       | tStream printStream)` | printStream.          |
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

        []{#printJsonOutput(com.google.common.collect.Multimap,java.io.PrintStream)}

        -   #### printJsonOutput

            ``` methodSignature
            public static void printJsonOutput​(com.google.common.collect.Multimap<String,​QueryTarget> targetsAndResults,
                                               PrintStream printStream)
                                        throws IOException
            ```

            ::: block
            Prints target and result map\'s json representation into
            printStream.
            :::

            [Parameters:]{.paramLabel}
            :   `targetsAndResults` - input to query result multi map
            :   `printStream` - print stream for output

            [Throws:]{.throwsLabel}
            :   `IOException` - in case of IO exception during json
                writing operation

        []{#printJsonOutput(java.util.Set,java.io.PrintStream)}

        -   #### printJsonOutput

            ``` methodSignature
            public static void printJsonOutput​(Set<QueryTarget> targets,
                                               PrintStream printStream)
                                        throws IOException
            ```

            ::: block
            Prints targets set json representation into printStream.
            :::

            [Parameters:]{.paramLabel}
            :   `targets` - set of query result
            :   `printStream` - print stream for output

            [Throws:]{.throwsLabel}
            :   `IOException` - in case of IO exception during json
                writing operation

        []{#print(com.google.common.collect.Multimap,java.io.PrintStream)}

        -   #### print

            ``` methodSignature
            public static void print​(com.google.common.collect.Multimap<String,​QueryTarget> targetsAndDependencies,
                                     PrintStream printStream)
            ```

            ::: block
            Prints target and dependencies map into printStream.
            :::

            [Parameters:]{.paramLabel}
            :   `targetsAndDependencies` - input to query result multi
                map
            :   `printStream` - print stream for output

        []{#print(java.util.Set,java.io.PrintStream)}

        -   #### print

            ``` methodSignature
            public static void print​(Set<QueryTarget> targets,
                                     PrintStream printStream)
            ```

            ::: block
            Prints target set into printStream.
            :::

            [Parameters:]{.paramLabel}
            :   `targets` - set of query result
            :   `printStream` - print stream for output

        []{#printShortDescription(com.facebook.buck.cli.Command,java.io.PrintStream)}

        -   #### printShortDescription

            ``` methodSignature
            public static void printShortDescription​(Command command,
                                                     PrintStream printStream)
            ```

            ::: block
            Prints short description of a given command into
            printStream.
            :::

            [Parameters:]{.paramLabel}
            :   `command` - CLI command
            :   `printStream` - print stream for output

        []{#maybePrintShowOutputWarning(com.facebook.buck.support.cli.config.CliConfig,com.facebook.buck.util.Ansi,com.facebook.buck.event.BuckEventBus)}

        -   #### maybePrintShowOutputWarning

            ``` methodSignature
            public static void maybePrintShowOutputWarning​(CliConfig cliConfig,
                                                           Ansi ansi,
                                                           BuckEventBus buckEventBus)
            ```

            ::: block
            Prints a warning to terminal about \--show-output being
            replaced by \--show-outputs if the warning is enabled in the
            buck config and the environment supports ANSI.
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
