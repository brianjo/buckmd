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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Enum DxStep.Option {#enum-dxstep.option .title title="Enum DxStep.Option"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[DxStep.Option](DxStep.Option.html "enum in com.facebook.buck.android")\>

    -   -   com.facebook.buck.android.DxStep.Option

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<DxStep.Option>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [DxStep](DxStep.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static enum DxStep.Option
        extends Enum<DxStep.Option>

    ::: block
    Options to pass to `dx`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `FORCE_JUMBO`                     | ::: block                         |
        |                                   | Force the dexer to emit jumbo     |
        |                                   | string references                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `NO_DESUGAR`                      | ::: block                         |
        |                                   | Disable java 8 desugaring when    |
        |                                   | running D8 dexing tool.           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `NO_LOCALS`                       | ::: block                         |
        |                                   | Run DX with the \--no-locals      |
        |                                   | flag.                             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `NO_OPTIMIZE`                     | ::: block                         |
        |                                   | Specify the `--no-optimize` flag  |
        |                                   | when running `dx`.                |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `RUN_IN_PROCESS`                  | ::: block                         |
        |                                   | Execute DX in-process instead of  |
        |                                   | fork/execing.                     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `USE_CUSTOM_DX_IF_AVAILABLE`      | ::: block                         |
        |                                   | See if the `buck.dx` property was |
        |                                   | specified, and if so, use the     |
        |                                   | executable that that points to    |
        |                                   | instead of the `dx` in the        |
        |                                   | user\'s Android SDK.              |
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
        | `                     | `                     | ::: block             |
        | static DxStep.Option` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `values()`            | ::: block             |
        | atic DxStep.Option[]` |                       | Returns an array      |
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

        []{#NO_OPTIMIZE}

        -   #### NO_OPTIMIZE

                public static final DxStep.Option NO_OPTIMIZE

            ::: block
            Specify the `--no-optimize` flag when running `dx`.
            :::

        []{#FORCE_JUMBO}

        -   #### FORCE_JUMBO

                public static final DxStep.Option FORCE_JUMBO

            ::: block
            Force the dexer to emit jumbo string references
            :::

        []{#USE_CUSTOM_DX_IF_AVAILABLE}

        -   #### USE_CUSTOM_DX_IF_AVAILABLE

                public static final DxStep.Option USE_CUSTOM_DX_IF_AVAILABLE

            ::: block
            See if the `buck.dx` property was specified, and if so, use
            the executable that that points to instead of the `dx` in
            the user\'s Android SDK.
            :::

        []{#RUN_IN_PROCESS}

        -   #### RUN_IN_PROCESS

                public static final DxStep.Option RUN_IN_PROCESS

            ::: block
            Execute DX in-process instead of fork/execing. This only
            works with custom dx.
            :::

        []{#NO_LOCALS}

        -   #### NO_LOCALS

                public static final DxStep.Option NO_LOCALS

            ::: block
            Run DX with the \--no-locals flag.
            :::

        []{#NO_DESUGAR}

        -   #### NO_DESUGAR

                public static final DxStep.Option NO_DESUGAR

            ::: block
            Disable java 8 desugaring when running D8 dexing tool.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static DxStep.Option[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (DxStep.Option c : DxStep.Option.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static DxStep.Option valueOf​(String name)
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
