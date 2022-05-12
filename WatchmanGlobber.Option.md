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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.io.impl](package-summary.html)
:::

## Enum WatchmanGlobber.Option {#enum-watchmanglobber.option .title title="Enum WatchmanGlobber.Option"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[WatchmanGlobber.Option](WatchmanGlobber.Option.html "enum in com.facebook.buck.skylark.io.impl")\>

    -   -   com.facebook.buck.skylark.io.impl.WatchmanGlobber.Option

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<WatchmanGlobber.Option>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [WatchmanGlobber](WatchmanGlobber.html "class in com.facebook.buck.skylark.io.impl")

    ------------------------------------------------------------------------

        public static enum WatchmanGlobber.Option
        extends Enum<WatchmanGlobber.Option>

    ::: block
    Watchman options to use when globbing.
    :::

    [See Also:]{.seeLabel}
    :   [`WatchmanGlobber.run(Collection, Collection, EnumSet)`](WatchmanGlobber.html#run(java.util.Collection,java.util.Collection,java.util.EnumSet))
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `EXCLUDE_DIRECTORIES`             | ::: block                         |
        |                                   | Do not return directories which   |
        |                                   | match include patterns.           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `EXCLUDE_SYMLINKS`                | ::: block                         |
        |                                   | Do not return symbolic links      |
        |                                   | which match include patterns.     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FORCE_CASE_SENSITIVE`            | ::: block                         |
        |                                   | Match path components exactly,    |
        |                                   | even on case-insensitive file     |
        |                                   | systems.                          |
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
        | `static Wa            | `                     | ::: block             |
        | tchmanGlobber.Option` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Watc          | `values()`            | ::: block             |
        | hmanGlobber.Option[]` |                       | Returns an array      |
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

        []{#EXCLUDE_DIRECTORIES}

        -   #### EXCLUDE_DIRECTORIES

                public static final WatchmanGlobber.Option EXCLUDE_DIRECTORIES

            ::: block
            Do not return directories which match include patterns.
            Symlinks referring to directories are still returned unless
            [`EXCLUDE_SYMLINKS`](#EXCLUDE_SYMLINKS) is also specified.

            This option corresponds to a [`type`
            expression](https://facebook.github.io/watchman/docs/expr/type.html)
            which excludes directories.
            :::

        []{#EXCLUDE_SYMLINKS}

        -   #### EXCLUDE_SYMLINKS

                public static final WatchmanGlobber.Option EXCLUDE_SYMLINKS

            ::: block
            Do not return symbolic links which match include patterns.
            Without this option, symbolic links are returned, regardless
            of their target.

            This option corresponds to a [`type`
            expression](https://facebook.github.io/watchman/docs/expr/type.html)
            which excludes symbolic links.
            :::

        []{#FORCE_CASE_SENSITIVE}

        -   #### FORCE_CASE_SENSITIVE

                public static final WatchmanGlobber.Option FORCE_CASE_SENSITIVE

            ::: block
            Match path components exactly, even on case-insensitive file
            systems.
            By default, whether or not patterns ignore case depends on
            [Watchman\'s default
            behavior](https://facebook.github.io/watchman/docs/cmd/query.html#case-sensitivity).

            This option affects both include patterns and exclude
            patterns.

            This option corresponds to the query\'s [`  case_sensitive`
            option](https://facebook.github.io/watchman/docs/cmd/query.html#case-sensitivity)
            to `true`.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static WatchmanGlobber.Option[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (WatchmanGlobber.Option c : WatchmanGlobber.Option.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static WatchmanGlobber.Option valueOf​(String name)
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
