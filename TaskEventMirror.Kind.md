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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.api](package-summary.html)
:::

## Enum TaskEventMirror.Kind {#enum-taskeventmirror.kind .title title="Enum TaskEventMirror.Kind"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[TaskEventMirror.Kind](TaskEventMirror.Kind.html "enum in com.facebook.buck.jvm.java.plugin.api")\>

    -   -   com.facebook.buck.jvm.java.plugin.api.TaskEventMirror.Kind

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<TaskEventMirror.Kind>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [TaskEventMirror](TaskEventMirror.html "class in com.facebook.buck.jvm.java.plugin.api")

    ------------------------------------------------------------------------

        public static enum TaskEventMirror.Kind
        extends Enum<TaskEventMirror.Kind>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `ANALYZE`                         | ::: block                         |
        |                                   | For events relating to elements   |
        |                                   | being analyzed for errors.        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ANNOTATION_PROCESSING`           | ::: block                         |
        |                                   | For events relating to overall    |
        |                                   | annotation processing.            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ANNOTATION_PROCESSING_ROUND`     | ::: block                         |
        |                                   | For events relating to an         |
        |                                   | individual annotation processing  |
        |                                   | round.                            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `COMPILATION`                     | ::: block                         |
        |                                   | Sent before parsing first source  |
        |                                   | file, and after writing the last  |
        |                                   | output file.                      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ENTER`                           | ::: block                         |
        |                                   | For events relating to elements   |
        |                                   | being entered.                    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `GENERATE`                        | ::: block                         |
        |                                   | For events relating to class      |
        |                                   | files being generated.            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PARSE`                           | ::: block                         |
        |                                   | For events related to the parsing |
        |                                   | of a file.                        |
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
        | `static               | `                     | ::: block             |
        | TaskEventMirror.Kind` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Ta            | `values()`            | ::: block             |
        | skEventMirror.Kind[]` |                       | Returns an array      |
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

        []{#PARSE}

        -   #### PARSE

                public static final TaskEventMirror.Kind PARSE

            ::: block
            For events related to the parsing of a file.
            :::

        []{#ENTER}

        -   #### ENTER

                public static final TaskEventMirror.Kind ENTER

            ::: block
            For events relating to elements being entered.
            :::

        []{#ANALYZE}

        -   #### ANALYZE

                public static final TaskEventMirror.Kind ANALYZE

            ::: block
            For events relating to elements being analyzed for errors.
            :::

        []{#GENERATE}

        -   #### GENERATE

                public static final TaskEventMirror.Kind GENERATE

            ::: block
            For events relating to class files being generated.
            :::

        []{#ANNOTATION_PROCESSING}

        -   #### ANNOTATION_PROCESSING

                public static final TaskEventMirror.Kind ANNOTATION_PROCESSING

            ::: block
            For events relating to overall annotation processing.
            :::

        []{#ANNOTATION_PROCESSING_ROUND}

        -   #### ANNOTATION_PROCESSING_ROUND

                public static final TaskEventMirror.Kind ANNOTATION_PROCESSING_ROUND

            ::: block
            For events relating to an individual annotation processing
            round.
            :::

        []{#COMPILATION}

        -   #### COMPILATION

                public static final TaskEventMirror.Kind COMPILATION

            ::: block
            Sent before parsing first source file, and after writing the
            last output file. This event is not sent when using
            `JavacTask#parse()`, `JavacTask#analyze()` or
            `  JavacTask#generate()`.
            :::

            [Since:]{.simpleTagLabel}
            :   9
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static TaskEventMirror.Kind[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (TaskEventMirror.Kind c : TaskEventMirror.Kind.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static TaskEventMirror.Kind valueOf​(String name)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
