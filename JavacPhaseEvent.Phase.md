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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.tracing](package-summary.html)
:::

## Enum JavacPhaseEvent.Phase {#enum-javacphaseevent.phase .title title="Enum JavacPhaseEvent.Phase"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[JavacPhaseEvent.Phase](JavacPhaseEvent.Phase.html "enum in com.facebook.buck.jvm.java.tracing")\>

    -   -   com.facebook.buck.jvm.java.tracing.JavacPhaseEvent.Phase

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<JavacPhaseEvent.Phase>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [JavacPhaseEvent](JavacPhaseEvent.html "class in com.facebook.buck.jvm.java.tracing")

    ------------------------------------------------------------------------

        public static enum JavacPhaseEvent.Phase
        extends Enum<JavacPhaseEvent.Phase>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `ANALYZE`                         | ::: block                         |
        |                                   | Analyze and transform the AST for |
        |                                   | a single type to prepare for code |
        |                                   | generation.                       |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ANNOTATION_PROCESSING`           | ::: block                         |
        |                                   | Overall annotation processing     |
        |                                   | phase, including all rounds.      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ANNOTATION_PROCESSING_ROUND`     | ::: block                         |
        |                                   | A single round of annotation      |
        |                                   | processing, including running the |
        |                                   | relevant processors, parsing any  |
        |                                   | source files they create, then    |
        |                                   | re-entering all previously parsed |
        |                                   | files into new symbol tables.     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ENTER`                           | ::: block                         |
        |                                   | Entering all parse trees into the |
        |                                   | compiler\'s symbol tables.        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `GENERATE`                        | ::: block                         |
        |                                   | Generate a class file for a       |
        |                                   | single type.                      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PARSE`                           | ::: block                         |
        |                                   | Parsing a single source file.     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `RUN_ANNOTATION_PROCESSORS`       | ::: block                         |
        |                                   | Just running the annotation       |
        |                                   | processors that are relevant to   |
        |                                   | the sources being compiled.       |
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
        | `static J             | `from                 |                       |
        | avacPhaseEvent.Phase` | String​(String value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static J             | `                     | ::: block             |
        | avacPhaseEvent.Phase` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Jav           | `values()`            | ::: block             |
        | acPhaseEvent.Phase[]` |                       | Returns an array      |
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

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, valueOf`

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

                public static final JavacPhaseEvent.Phase PARSE

            ::: block
            Parsing a single source file. Filename will be in the args.
            :::

        []{#ENTER}

        -   #### ENTER

                public static final JavacPhaseEvent.Phase ENTER

            ::: block
            Entering all parse trees into the compiler\'s symbol tables.
            All filenames will be in the args.
            :::

        []{#ANNOTATION_PROCESSING}

        -   #### ANNOTATION_PROCESSING

                public static final JavacPhaseEvent.Phase ANNOTATION_PROCESSING

            ::: block
            Overall annotation processing phase, including all rounds.
            No args.
            :::

        []{#ANNOTATION_PROCESSING_ROUND}

        -   #### ANNOTATION_PROCESSING_ROUND

                public static final JavacPhaseEvent.Phase ANNOTATION_PROCESSING_ROUND

            ::: block
            A single round of annotation processing, including running
            the relevant processors, parsing any source files they
            create, then re-entering all previously parsed files into
            new symbol tables. Round number and whether it\'s the last
            round will be in the args.
            :::

        []{#RUN_ANNOTATION_PROCESSORS}

        -   #### RUN_ANNOTATION_PROCESSORS

                public static final JavacPhaseEvent.Phase RUN_ANNOTATION_PROCESSORS

            ::: block
            Just running the annotation processors that are relevant to
            the sources being compiled. No args.
            :::

        []{#ANALYZE}

        -   #### ANALYZE

                public static final JavacPhaseEvent.Phase ANALYZE

            ::: block
            Analyze and transform the AST for a single type to prepare
            for code generation. Source file and type being analyzed
            will be in the args.
            :::

        []{#GENERATE}

        -   #### GENERATE

                public static final JavacPhaseEvent.Phase GENERATE

            ::: block
            Generate a class file for a single type. Source file and
            type being generated will be in the args.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static JavacPhaseEvent.Phase[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (JavacPhaseEvent.Phase c : JavacPhaseEvent.Phase.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static JavacPhaseEvent.Phase valueOf​(String name)
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

        []{#fromString(java.lang.String)}

        -   #### fromString

            ``` methodSignature
            public static JavacPhaseEvent.Phase fromString​(String value)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Enum<JavacPhaseEvent.Phase>`
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
