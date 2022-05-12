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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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

## Enum ExitCode {#enum-exitcode .title title="Enum ExitCode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ExitCode](ExitCode.html "enum in com.facebook.buck.util")\>

    -   -   com.facebook.buck.util.ExitCode

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ExitCode>`

    ------------------------------------------------------------------------

        public enum ExitCode
        extends Enum<ExitCode>

    ::: block
    ExitCode class defines Buck binary protocol, i.e. exit codes that
    Buck can report to a running shell. In addition to exit codes
    defined below, we have to honor following conventions.
    Buck bootstrapper must conform to the protocol, i.e. properly
    implement FATAL_BOOTSTRAP

    Exit codes for interrupts do follow POSIX convention, i.e. 128 +
    SIGNAL_CODE, i.e SIGINT is returned as 128 + 2 = 130

    Exit codes 1-9 are reserved for non-fatal errors, like build errors

    Exit codes 10-19 are reserved for fatal errors, like unexpected
    runtime exceptions

    Binary protocol is open to extension but closed to modification.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `BUILD_ERROR`                     | ::: block                         |
        |                                   | Build resulted in user-specific   |
        |                                   | error                             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `BUSY`                            | ::: block                         |
        |                                   | Buck daemon is busy processing    |
        |                                   | another command                   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `COMMANDLINE_ERROR`               | ::: block                         |
        |                                   | User supplied incorrect command   |
        |                                   | line options                      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FATAL_BOOTSTRAP`                 | ::: block                         |
        |                                   | Non-recoverable error in Buck     |
        |                                   | bootstrapper                      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FATAL_DISK_FULL`                 | ::: block                         |
        |                                   | No space on device                |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FATAL_GENERIC`                   | ::: block                         |
        |                                   | Generic Buck-internal             |
        |                                   | non-recoverable error             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FATAL_IO`                        | ::: block                         |
        |                                   | Non-recoverable generic I/0 error |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FATAL_OOM`                       | ::: block                         |
        |                                   | Non-recoverable OutOfMemory error |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FIX_FAILED`                      | ::: block                         |
        |                                   | Indicates that the buck fix       |
        |                                   | script returned a non-zero exit   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `NOTHING_TO_DO`                   | ::: block                         |
        |                                   | There is nothing to build or      |
        |                                   | evaluate for the command          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PARSE_ERROR`                     | ::: block                         |
        |                                   | There was build file parsing or   |
        |                                   | graph construction error          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `RUN_ERROR`                       | ::: block                         |
        |                                   | Running a binary or installing    |
        |                                   | binary to a device has failed     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SIGNAL_INTERRUPT`                | ::: block                         |
        |                                   | Command was interrupted (Ctrl +   |
        |                                   | C)                                |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SUCCESS`                         | ::: block                         |
        |                                   | Buck command completed            |
        |                                   | successfully                      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `TEST_ERROR`                      | ::: block                         |
        |                                   | Test run had user-specific test   |
        |                                   | errors                            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `TEST_NOTHING`                    | ::: block                         |
        |                                   | There was no tests found to run   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getCode()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isFatal()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ExitCode`     | `map​(int code)`       | ::: block             |
        |                       |                       | Map integer value     |
        |                       |                       | received from custom  |
        |                       |                       | toolchain subcall to  |
        |                       |                       | one of appropriate    |
        |                       |                       | ExitCode values.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ExitCode`     | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ExitCode[]`   | `values()`            | ::: block             |
        |                       |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#SUCCESS}

        -   #### SUCCESS

                public static final ExitCode SUCCESS

            ::: block
            Buck command completed successfully
            :::

        []{#BUILD_ERROR}

        -   #### BUILD_ERROR

                public static final ExitCode BUILD_ERROR

            ::: block
            Build resulted in user-specific error
            :::

        []{#BUSY}

        -   #### BUSY

                public static final ExitCode BUSY

            ::: block
            Buck daemon is busy processing another command
            :::

        []{#COMMANDLINE_ERROR}

        -   #### COMMANDLINE_ERROR

                public static final ExitCode COMMANDLINE_ERROR

            ::: block
            User supplied incorrect command line options
            :::

        []{#NOTHING_TO_DO}

        -   #### NOTHING_TO_DO

                public static final ExitCode NOTHING_TO_DO

            ::: block
            There is nothing to build or evaluate for the command
            :::

        []{#PARSE_ERROR}

        -   #### PARSE_ERROR

                public static final ExitCode PARSE_ERROR

            ::: block
            There was build file parsing or graph construction error
            :::

        []{#RUN_ERROR}

        -   #### RUN_ERROR

                public static final ExitCode RUN_ERROR

            ::: block
            Running a binary or installing binary to a device has failed
            :::

        []{#FATAL_GENERIC}

        -   #### FATAL_GENERIC

                public static final ExitCode FATAL_GENERIC

            ::: block
            Generic Buck-internal non-recoverable error
            :::

        []{#FATAL_BOOTSTRAP}

        -   #### FATAL_BOOTSTRAP

                public static final ExitCode FATAL_BOOTSTRAP

            ::: block
            Non-recoverable error in Buck bootstrapper
            :::

        []{#FATAL_OOM}

        -   #### FATAL_OOM

                public static final ExitCode FATAL_OOM

            ::: block
            Non-recoverable OutOfMemory error
            :::

        []{#FATAL_IO}

        -   #### FATAL_IO

                public static final ExitCode FATAL_IO

            ::: block
            Non-recoverable generic I/0 error
            :::

        []{#FATAL_DISK_FULL}

        -   #### FATAL_DISK_FULL

                public static final ExitCode FATAL_DISK_FULL

            ::: block
            No space on device
            :::

        []{#FIX_FAILED}

        -   #### FIX_FAILED

                public static final ExitCode FIX_FAILED

            ::: block
            Indicates that the buck fix script returned a non-zero exit
            :::

        []{#TEST_ERROR}

        -   #### TEST_ERROR

                public static final ExitCode TEST_ERROR

            ::: block
            Test run had user-specific test errors
            :::

        []{#TEST_NOTHING}

        -   #### TEST_NOTHING

                public static final ExitCode TEST_NOTHING

            ::: block
            There was no tests found to run
            :::

        []{#SIGNAL_INTERRUPT}

        -   #### SIGNAL_INTERRUPT

                public static final ExitCode SIGNAL_INTERRUPT

            ::: block
            Command was interrupted (Ctrl + C)
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ExitCode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ExitCode c : ExitCode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ExitCode valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#getCode()}

        -   #### getCode

            ``` methodSignature
            public int getCode()
            ```

            [Returns:]{.returnLabel}
            :   integer value of the exit code

        []{#isFatal()}

        -   #### isFatal

            ``` methodSignature
            public boolean isFatal()
            ```

            [Returns:]{.returnLabel}
            :   true if error is Buck internal non-recoverable failure

        []{#map(int)}

        -   #### map

            ``` methodSignature
            public static ExitCode map​(int code)
            ```

            ::: block
            Map integer value received from custom toolchain subcall to
            one of appropriate ExitCode values. This function is for
            backwards compatibility only, please construct ExitCode
            directly instead
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
