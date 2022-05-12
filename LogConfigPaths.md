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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class LogConfigPaths {#class-logconfigpaths .title title="Class LogConfigPaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.LogConfigPaths

::: description
-   

    ------------------------------------------------------------------------

        public class LogConfigPaths
        extends Object

    ::: block
    Utility class containing constants for logging configuration paths.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `                     | ::: block             |
        |                       | BUCK_CONFIG_STRING_TE | System property       |
        |                       | MPLATE_FILE_PROPERTY` | holding the path to   |
        |                       |                       | the                   |
        |                       |                       | logging.properties.st |
        |                       |                       | file in the Buck      |
        |                       |                       | repo.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `LOCAL_PATH`          | ::: block             |
        |                       |                       | The path to the       |
        |                       |                       | per-project local     |
        |                       |                       | (git ignored)         |
        |                       |                       | logging.properties    |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `MAIN_PATH`           | ::: block             |
        | tatic Optional<Path>` |                       | If present, the path  |
        |                       |                       | to the                |
        |                       |                       | logging.properties.st |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `PROJECT_PATH`        | ::: block             |
        |                       |                       | The path to the       |
        |                       |                       | per-project           |
        |                       |                       | logging.properties    |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#BUCK_CONFIG_STRING_TEMPLATE_FILE_PROPERTY}

        -   #### BUCK_CONFIG_STRING_TEMPLATE_FILE_PROPERTY

                public static final String BUCK_CONFIG_STRING_TEMPLATE_FILE_PROPERTY

            ::: block
            System property holding the path to the
            logging.properties.st file in the Buck repo.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.log.LogConfigPaths.BUCK_CONFIG_STRING_TEMPLATE_FILE_PROPERTY)

        []{#MAIN_PATH}

        -   #### MAIN_PATH

                public static final Optional<Path> MAIN_PATH

            ::: block
            If present, the path to the logging.properties.st file.
            :::

        []{#PROJECT_PATH}

        -   #### PROJECT_PATH

                public static final Path PROJECT_PATH

            ::: block
            The path to the per-project logging.properties file.
            :::

        []{#LOCAL_PATH}

        -   #### LOCAL_PATH

                public static final Path LOCAL_PATH

            ::: block
            The path to the per-project local (git ignored)
            logging.properties file.
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
