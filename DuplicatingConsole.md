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

## Class DuplicatingConsole {#class-duplicatingconsole .title title="Class DuplicatingConsole"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.Console](Console.html "class in com.facebook.buck.util")

    -   -   com.facebook.buck.util.DuplicatingConsole

::: description
-   

    ------------------------------------------------------------------------

        public class DuplicatingConsole
        extends Console

    ::: block
    Manages a Duplicate Console so that console actions can be
    replicated across to another console.
    Example use case is to duplicate a console that writes to system
    stdout/stderr to a Log file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                          Description
          ------------------------------------ -------------
          `DuplicatingConsole​(Console main)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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
        | `void`                | `setDuplicatingCo     |                       |
        |                       | nsole​(Optional<Consol |                       |
        |                       | e> duplicateConsole)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.Console}

            ### Methods inherited from class com.facebook.buck.util.[Console](Console.html "class in com.facebook.buck.util")

            `createNullConsole, getAnsi, getStdErr, getStdOut, getVerbosity`

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

        []{#<init>(com.facebook.buck.util.Console)}

        -   #### DuplicatingConsole

                public DuplicatingConsole​(Console main)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setDuplicatingConsole(java.util.Optional)}

        -   #### setDuplicatingConsole

            ``` methodSignature
            public void setDuplicatingConsole​(Optional<Console> duplicateConsole)
            ```

        []{#printSuccess(java.lang.String)}

        -   #### printSuccess

            ``` methodSignature
            public void printSuccess​(String successMessage)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `printSuccess` in class `Console`

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
            [Description copied from
            class: `Console`]{.descfrmTypeLabel}
            :::

            ::: block
            Prints a formatted success message. {@see
            #printSuccess(String)}
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `printSuccess` in class `Console`

        []{#printErrorText(java.lang.String)}

        -   #### printErrorText

            ``` methodSignature
            public void printErrorText​(String message)
            ```

            ::: block
            [Description copied from
            class: `Console`]{.descfrmTypeLabel}
            :::

            ::: block
            Prints an error message to stderr that will be highlighted
            in red if stderr is a tty.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `printErrorText` in class `Console`

        []{#printErrorText(java.lang.String,java.lang.Object...)}

        -   #### printErrorText

            ``` methodSignature
            public void printErrorText​(String message,
                                       Object... args)
            ```

            ::: block
            [Description copied from
            class: `Console`]{.descfrmTypeLabel}
            :::

            ::: block
            Prints a formatted error message. {@see
            #printErrorText(String)}
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `printErrorText` in class `Console`

        []{#printBuildFailure(java.lang.String)}

        -   #### printBuildFailure

            ``` methodSignature
            public void printBuildFailure​(String failureMessage)
            ```

            ::: block
            [Description copied from
            class: `Console`]{.descfrmTypeLabel}
            :::

            ::: block
            Prints an error message prefixed with `BUILD FAILED` to
            stderr that will be highlighted in red if stderr is a tty.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `printBuildFailure` in class `Console`

        []{#printFailure(java.lang.String)}

        -   #### printFailure

            ``` methodSignature
            public void printFailure​(String failureMessage)
            ```

            ::: block
            [Description copied from
            class: `Console`]{.descfrmTypeLabel}
            :::

            ::: block
            Prints error message to console in red, also logs stacktrace
            but does not display it
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `printFailure` in class `Console`
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
