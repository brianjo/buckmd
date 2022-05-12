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

## Class Console {#class-console .title title="Class Console"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.Console

::: description
-   

    Direct Known Subclasses:
    :   `DuplicatingConsole`

    ------------------------------------------------------------------------

        public class Console
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                              Description
          -------------------------------------------------------------------------------------------------------- -------------
          `Console​(Verbosity verbosity,        PrintStream stdOut,        PrintStream stdErr,        Ansi ansi)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Console`      | `createNullConsole()` | ::: block             |
        |                       |                       | Returns a             |
        |                       |                       | [`Console`](Conso     |
        |                       |                       | le.html "class in com |
        |                       |                       | .facebook.buck.util") |
        |                       |                       | that simply discards  |
        |                       |                       | written bytes.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ansi`                | `getAnsi()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dirty                | `getStdErr()`         |                       |
        | PrintStreamDecorator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dirty                | `getStdOut()`         |                       |
        | PrintStreamDecorator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Verbosity`           | `getVerbosity()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printBuildFailure​(St | ::: block             |
        |                       | ring failureMessage)` | Prints an error       |
        |                       |                       | message prefixed with |
        |                       |                       | `BUILD FAILED` to     |
        |                       |                       | stderr that will be   |
        |                       |                       | highlighted in red if |
        |                       |                       | stderr is a tty.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printError           | ::: block             |
        |                       | Text​(String message)` | Prints an error       |
        |                       |                       | message to stderr     |
        |                       |                       | that will be          |
        |                       |                       | highlighted in red if |
        |                       |                       | stderr is a tty.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printErrorText​(Stri  | ::: block             |
        |                       | ng message,           | Prints a formatted    |
        |                       |      Object... args)` | error message.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printFailure​(St      | ::: block             |
        |                       | ring failureMessage)` | Prints error message  |
        |                       |                       | to console in red,    |
        |                       |                       | also logs stacktrace  |
        |                       |                       | but does not display  |
        |                       |                       | it                    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printSuccess​(St      |                       |
        |                       | ring successMessage)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `p                    | ::: block             |
        |                       | rintSuccess​(String su | Prints a formatted    |
        |                       | ccessMessage,         | success message.      |
        |                       |      Object... args)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.util.Verbosity,java.io.PrintStream,java.io.PrintStream,com.facebook.buck.util.Ansi)}

        -   #### Console

                public Console​(Verbosity verbosity,
                               PrintStream stdOut,
                               PrintStream stdErr,
                               Ansi ansi)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createNullConsole()}

        -   #### createNullConsole

            ``` methodSignature
            public static Console createNullConsole()
            ```

            ::: block
            Returns a
            [`Console`](Console.html "class in com.facebook.buck.util")
            that simply discards written bytes.
            :::

        []{#getVerbosity()}

        -   #### getVerbosity

            ``` methodSignature
            public Verbosity getVerbosity()
            ```

        []{#getAnsi()}

        -   #### getAnsi

            ``` methodSignature
            public Ansi getAnsi()
            ```

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            public DirtyPrintStreamDecorator getStdOut()
            ```

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            public DirtyPrintStreamDecorator getStdErr()
            ```

        []{#printSuccess(java.lang.String)}

        -   #### printSuccess

            ``` methodSignature
            public void printSuccess​(String successMessage)
            ```

            [Parameters:]{.paramLabel}
            :   `successMessage` - single line of text without a
                trailing newline. If stdErr is attached to a terminal,
                then this will append an ANSI reset escape sequence
                followed by a newline.

        []{#printSuccess(java.lang.String,java.lang.Object...)}

        -   #### printSuccess

            ``` methodSignature
            public void printSuccess​(String successMessage,
                                     Object... args)
            ```

            ::: block
            Prints a formatted success message. {@see
            #printSuccess(String)}
            :::

        []{#printErrorText(java.lang.String)}

        -   #### printErrorText

            ``` methodSignature
            public void printErrorText​(String message)
            ```

            ::: block
            Prints an error message to stderr that will be highlighted
            in red if stderr is a tty.
            :::

        []{#printErrorText(java.lang.String,java.lang.Object...)}

        -   #### printErrorText

            ``` methodSignature
            public void printErrorText​(String message,
                                       Object... args)
            ```

            ::: block
            Prints a formatted error message. {@see
            #printErrorText(String)}
            :::

        []{#printBuildFailure(java.lang.String)}

        -   #### printBuildFailure

            ``` methodSignature
            public void printBuildFailure​(String failureMessage)
            ```

            ::: block
            Prints an error message prefixed with `BUILD FAILED` to
            stderr that will be highlighted in red if stderr is a tty.
            :::

        []{#printFailure(java.lang.String)}

        -   #### printFailure

            ``` methodSignature
            public void printFailure​(String failureMessage)
            ```

            ::: block
            Prints error message to console in red, also logs stacktrace
            but does not display it
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
