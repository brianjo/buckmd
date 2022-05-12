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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Enum GroupedSource.Type {#enum-groupedsource.type .title title="Enum GroupedSource.Type"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[GroupedSource.Type](GroupedSource.Type.html "enum in com.facebook.buck.apple")\>

    -   -   com.facebook.buck.apple.GroupedSource.Type

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<GroupedSource.Type>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [GroupedSource](GroupedSource.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        public static enum GroupedSource.Type
        extends Enum<GroupedSource.Type>

    ::: block
    The type of grouped source entry this object represents.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `IGNORED_SOURCE`                  | ::: block                         |
        |                                   | A single                          |
        |                                   | [`SourcePath`](../core/sourcepath |
        |                                   | /SourcePath.html "interface in co |
        |                                   | m.facebook.buck.core.sourcepath") |
        |                                   | that shouldn\'t be included in    |
        |                                   | the build phase.                  |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PRIVATE_HEADER`                  | ::: block                         |
        |                                   | A single                          |
        |                                   | [`SourcePath`](../core/sourcepath |
        |                                   | /SourcePath.html "interface in co |
        |                                   | m.facebook.buck.core.sourcepath") |
        |                                   | representing a private header     |
        |                                   | file.                             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PUBLIC_HEADER`                   | ::: block                         |
        |                                   | A single                          |
        |                                   | [`SourcePath`](../core/sourcepath |
        |                                   | /SourcePath.html "interface in co |
        |                                   | m.facebook.buck.core.sourcepath") |
        |                                   | representing a public header      |
        |                                   | file.                             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SOURCE_GROUP`                    | ::: block                         |
        |                                   | A source group (group name and    |
        |                                   | one or more GroupedSource         |
        |                                   | objects).                         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SOURCE_WITH_FLAGS`               | ::: block                         |
        |                                   | A single                          |
        |                                   | [`Sourc                           |
        |                                   | eWithFlags`](../core/sourcepath/S |
        |                                   | ourceWithFlags.html "class in com |
        |                                   | .facebook.buck.core.sourcepath"). |
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
        | `stati                | `                     | ::: block             |
        | c GroupedSource.Type` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `values()`            | ::: block             |
        | GroupedSource.Type[]` |                       | Returns an array      |
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

        []{#SOURCE_WITH_FLAGS}

        -   #### SOURCE_WITH_FLAGS

                public static final GroupedSource.Type SOURCE_WITH_FLAGS

            ::: block
            A single
            [`SourceWithFlags`](../core/sourcepath/SourceWithFlags.html "class in com.facebook.buck.core.sourcepath").
            :::

        []{#IGNORED_SOURCE}

        -   #### IGNORED_SOURCE

                public static final GroupedSource.Type IGNORED_SOURCE

            ::: block
            A single
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            that shouldn\'t be included in the build phase.
            :::

        []{#PUBLIC_HEADER}

        -   #### PUBLIC_HEADER

                public static final GroupedSource.Type PUBLIC_HEADER

            ::: block
            A single
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            representing a public header file.
            :::

        []{#PRIVATE_HEADER}

        -   #### PRIVATE_HEADER

                public static final GroupedSource.Type PRIVATE_HEADER

            ::: block
            A single
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            representing a private header file.
            :::

        []{#SOURCE_GROUP}

        -   #### SOURCE_GROUP

                public static final GroupedSource.Type SOURCE_GROUP

            ::: block
            A source group (group name and one or more GroupedSource
            objects).
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static GroupedSource.Type[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (GroupedSource.Type c : GroupedSource.Type.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static GroupedSource.Type valueOf​(String name)
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
