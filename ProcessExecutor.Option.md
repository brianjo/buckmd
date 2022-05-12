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

## Enum ProcessExecutor.Option {#enum-processexecutor.option .title title="Enum ProcessExecutor.Option"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ProcessExecutor.Option](ProcessExecutor.Option.html "enum in com.facebook.buck.util")\>

    -   -   com.facebook.buck.util.ProcessExecutor.Option

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ProcessExecutor.Option>`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [ProcessExecutor](ProcessExecutor.html "interface in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static enum ProcessExecutor.Option
        extends Enum<ProcessExecutor.Option>

    ::: block
    Options for
    [`ProcessExecutor.launchAndExecute(ProcessExecutorParams, Set, Optional,  Optional, Optional)`](ProcessExecutor.html#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `EXPECTING_STD_ERR`               |                                   |
        +-----------------------------------+-----------------------------------+
        | `EXPECTING_STD_OUT`               | ::: block                         |
        |                                   | If set, will not highlight output |
        |                                   | to stdout or stderr when          |
        |                                   | printing.                         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `IS_SILENT`                       | ::: block                         |
        |                                   | If set, do not write output to    |
        |                                   | stdout or stderr.                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PRINT_STD_ERR`                   |                                   |
        +-----------------------------------+-----------------------------------+
        | `PRINT_STD_OUT`                   |                                   |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Pr            | `                     | ::: block             |
        | ocessExecutor.Option` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Proc          | `values()`            | ::: block             |
        | essExecutor.Option[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#PRINT_STD_OUT}

        -   #### PRINT_STD_OUT

                public static final ProcessExecutor.Option PRINT_STD_OUT

        []{#PRINT_STD_ERR}

        -   #### PRINT_STD_ERR

                public static final ProcessExecutor.Option PRINT_STD_ERR

        []{#EXPECTING_STD_OUT}

        -   #### EXPECTING_STD_OUT

                public static final ProcessExecutor.Option EXPECTING_STD_OUT

            ::: block
            If set, will not highlight output to stdout or stderr when
            printing.
            :::

        []{#EXPECTING_STD_ERR}

        -   #### EXPECTING_STD_ERR

                public static final ProcessExecutor.Option EXPECTING_STD_ERR

        []{#IS_SILENT}

        -   #### IS_SILENT

                public static final ProcessExecutor.Option IS_SILENT

            ::: block
            If set, do not write output to stdout or stderr. However, if
            the process exits with a non-zero exit code, then the stdout
            and stderr from the process will be presented to the user to
            aid in debugging.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ProcessExecutor.Option[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ProcessExecutor.Option c : ProcessExecutor.Option.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ProcessExecutor.Option valueOf​(String name)
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
