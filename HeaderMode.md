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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Enum HeaderMode {#enum-headermode .title title="Enum HeaderMode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[HeaderMode](HeaderMode.html "enum in com.facebook.buck.cxx.toolchain")\>

    -   -   com.facebook.buck.cxx.toolchain.HeaderMode

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `Serializable`, `Comparable<HeaderMode>`

    ------------------------------------------------------------------------

        public enum HeaderMode
        extends Enum<HeaderMode>
        implements FlavorConvertible
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `HEADER_MAP_ONLY`                 | ::: block                         |
        |                                   | Creates the header map that       |
        |                                   | references the headers directly   |
        |                                   | in the source tree.               |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SYMLINK_TREE_ONLY`               | ::: block                         |
        |                                   | Creates the tree of symbolic      |
        |                                   | links of headers.                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SYMLINK_TREE_WITH_HEADER_MAP`    | ::: block                         |
        |                                   | Creates the tree of symbolic      |
        |                                   | links of headers and creates the  |
        |                                   | header map that references the    |
        |                                   | symbolic links to the headers.    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SYM                              | ::: block                         |
        | LINK_TREE_WITH_HEADERS_MODULEMAP` | Creates the tree of symbolic      |
        |                                   | links of headers and creates a    |
        |                                   | module map that references the    |
        |                                   | symbolic links to the headers.    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SYMLINK_TRE                      | ::: block                         |
        | E_WITH_UMBRELLA_HEADER_MODULEMAP` | Creates the tree of symbolic      |
        |                                   | links of headers and creates a    |
        |                                   | module map that references the    |
        |                                   | symbolic links to the headers.    |
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
        | `static HeaderMode`   | `forM                 | ::: block             |
        |                       | oduleMapMode​(ModuleMa | Returns the           |
        |                       | pMode moduleMapMode)` | appropriate header    |
        |                       |                       | mode for module map   |
        |                       |                       | mode.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `includesModuleMap()` | ::: block             |
        |                       |                       | Returns whether or    |
        |                       |                       | not the header mode   |
        |                       |                       | will include a module |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static HeaderMode`   | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static HeaderMode[]` | `values()`            | ::: block             |
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

        []{#SYMLINK_TREE_ONLY}

        -   #### SYMLINK_TREE_ONLY

                public static final HeaderMode SYMLINK_TREE_ONLY

            ::: block
            Creates the tree of symbolic links of headers.
            :::

        []{#HEADER_MAP_ONLY}

        -   #### HEADER_MAP_ONLY

                public static final HeaderMode HEADER_MAP_ONLY

            ::: block
            Creates the header map that references the headers directly
            in the source tree.
            :::

        []{#SYMLINK_TREE_WITH_HEADER_MAP}

        -   #### SYMLINK_TREE_WITH_HEADER_MAP

                public static final HeaderMode SYMLINK_TREE_WITH_HEADER_MAP

            ::: block
            Creates the tree of symbolic links of headers and creates
            the header map that references the symbolic links to the
            headers.
            :::

        []{#SYMLINK_TREE_WITH_HEADERS_MODULEMAP}

        -   #### SYMLINK_TREE_WITH_HEADERS_MODULEMAP

                public static final HeaderMode SYMLINK_TREE_WITH_HEADERS_MODULEMAP

            ::: block
            Creates the tree of symbolic links of headers and creates a
            module map that references the symbolic links to the
            headers. The generated module map will refer to explicit
            headers.
            :::

        []{#SYMLINK_TREE_WITH_UMBRELLA_HEADER_MODULEMAP}

        -   #### SYMLINK_TREE_WITH_UMBRELLA_HEADER_MODULEMAP

                public static final HeaderMode SYMLINK_TREE_WITH_UMBRELLA_HEADER_MODULEMAP

            ::: block
            Creates the tree of symbolic links of headers and creates a
            module map that references the symbolic links to the
            headers. The generated module map will refer to an umbrella
            header, with the same name as the library.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static HeaderMode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (HeaderMode c : HeaderMode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static HeaderMode valueOf​(String name)
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

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#forModuleMapMode(com.facebook.buck.apple.clang.ModuleMapMode)}

        -   #### forModuleMapMode

            ``` methodSignature
            public static HeaderMode forModuleMapMode​(ModuleMapMode moduleMapMode)
            ```

            ::: block
            Returns the appropriate header mode for module map mode.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleMapMode` - The module map mode to convert.

            [Returns:]{.returnLabel}
            :   The equivalent header mode.

        []{#includesModuleMap()}

        -   #### includesModuleMap

            ``` methodSignature
            public boolean includesModuleMap()
            ```

            ::: block
            Returns whether or not the header mode will include a module
            map.
            :::

            [Returns:]{.returnLabel}
            :   true if the header mode will include a module map,
                otherwise false.
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
