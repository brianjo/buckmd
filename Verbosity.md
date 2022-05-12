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

## Enum Verbosity {#enum-verbosity .title title="Enum Verbosity"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[Verbosity](Verbosity.html "enum in com.facebook.buck.util")\>

    -   -   com.facebook.buck.util.Verbosity

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<Verbosity>`

    ------------------------------------------------------------------------

        public enum Verbosity
        extends Enum<Verbosity>

    ::: block
    An indication of how verbose Buck should be. Enum values are in
    order from least to most verbose.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `ALL`                             | ::: block                         |
        |                                   | If the command being executed has |
        |                                   | its own `--verbose` option or     |
        |                                   | equivalent, it should be used.    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `BINARY_OUTPUTS`                  | ::: block                         |
        |                                   | Print extra output from generated |
        |                                   | binaries and tests being run, but |
        |                                   | nothing else.                     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `COMMANDS`                        | ::: block                         |
        |                                   | Print the command being executed, |
        |                                   | but do not print its output.      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `COMMANDS_AND_OUTPUT`             | ::: block                         |
        |                                   | Print the command being executed  |
        |                                   | followed by its output.           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `COMMANDS_AND_SPECIAL_OUTPUT`     | ::: block                         |
        |                                   | Commands plus the output from     |
        |                                   | some select commands of interest. |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SILENT`                          | ::: block                         |
        |                                   | Do not print anything to the      |
        |                                   | console.                          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `STANDARD_INFORMATION`            | ::: block                         |
        |                                   | Prints out the bare minimum       |
        |                                   | required information, such as     |
        |                                   | errors from build steps.          |
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
        | `boolean`             | `isSilent()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldPrintBi        |                       |
        |                       | naryRunInformation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | shouldPrintCommand()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldPrintOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldPrintS         |                       |
        |                       | electCommandOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldPrintS         |                       |
        |                       | tandardInformation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldUseVerbos      |                       |
        |                       | ityFlagIfAvailable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Verbosity`    | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Verbosity[]`  | `values()`            | ::: block             |
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

        []{#SILENT}

        -   #### SILENT

                public static final Verbosity SILENT

            ::: block
            Do not print anything to the console.
            :::

        []{#STANDARD_INFORMATION}

        -   #### STANDARD_INFORMATION

                public static final Verbosity STANDARD_INFORMATION

            ::: block
            Prints out the bare minimum required information, such as
            errors from build steps.
            :::

        []{#BINARY_OUTPUTS}

        -   #### BINARY_OUTPUTS

                public static final Verbosity BINARY_OUTPUTS

            ::: block
            Print extra output from generated binaries and tests being
            run, but nothing else.
            :::

        []{#COMMANDS}

        -   #### COMMANDS

                public static final Verbosity COMMANDS

            ::: block
            Print the command being executed, but do not print its
            output.
            :::

        []{#COMMANDS_AND_SPECIAL_OUTPUT}

        -   #### COMMANDS_AND_SPECIAL_OUTPUT

                public static final Verbosity COMMANDS_AND_SPECIAL_OUTPUT

            ::: block
            Commands plus the output from some select commands of
            interest.
            :::

        []{#COMMANDS_AND_OUTPUT}

        -   #### COMMANDS_AND_OUTPUT

                public static final Verbosity COMMANDS_AND_OUTPUT

            ::: block
            Print the command being executed followed by its output.
            :::

        []{#ALL}

        -   #### ALL

                public static final Verbosity ALL

            ::: block
            If the command being executed has its own `--verbose` option
            or equivalent, it should be used.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static Verbosity[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (Verbosity c : Verbosity.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static Verbosity valueOf​(String name)
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

        []{#isSilent()}

        -   #### isSilent

            ``` methodSignature
            public boolean isSilent()
            ```

        []{#shouldPrintStandardInformation()}

        -   #### shouldPrintStandardInformation

            ``` methodSignature
            public boolean shouldPrintStandardInformation()
            ```

        []{#shouldPrintBinaryRunInformation()}

        -   #### shouldPrintBinaryRunInformation

            ``` methodSignature
            public boolean shouldPrintBinaryRunInformation()
            ```

        []{#shouldPrintCommand()}

        -   #### shouldPrintCommand

            ``` methodSignature
            public boolean shouldPrintCommand()
            ```

        []{#shouldPrintSelectCommandOutput()}

        -   #### shouldPrintSelectCommandOutput

            ``` methodSignature
            public boolean shouldPrintSelectCommandOutput()
            ```

        []{#shouldPrintOutput()}

        -   #### shouldPrintOutput

            ``` methodSignature
            public boolean shouldPrintOutput()
            ```

        []{#shouldUseVerbosityFlagIfAvailable()}

        -   #### shouldUseVerbosityFlagIfAvailable

            ``` methodSignature
            public boolean shouldUseVerbosityFlagIfAvailable()
            ```

            [Returns:]{.returnLabel}
            :   `true` if the command being executed should use its own
                `--verbose` argument (or equivalent) for this Verbosity
                level
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
