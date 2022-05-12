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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetpattern](package-summary.html)
:::

## Class BuildTargetLanguageConstants {#class-buildtargetlanguageconstants .title title="Class BuildTargetLanguageConstants"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants

::: description
-   

    ------------------------------------------------------------------------

        public final class BuildTargetLanguageConstants
        extends Object

    ::: block
    Defines symbols which are a part of the build target and build
    target pattern formats
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static char`         | `FLAVOR_DELIMITER`    | ::: block             |
        |                       |                       | Symbol that delimits  |
        |                       |                       | flavors specified     |
        |                       |                       | after FLAVOR_SYMBOL   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static char`         | `FLAVOR_SYMBOL`       | ::: block             |
        |                       |                       | Symbol that           |
        |                       |                       | represents flavor     |
        |                       |                       | part of a build       |
        |                       |                       | target                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static char`         | `PATH_SYMBOL`         | ::: block             |
        |                       |                       | Delimiter that splits |
        |                       |                       | path to a package     |
        |                       |                       | root in the pattern   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `RECURSIVE_SYMBOL`    | ::: block             |
        |                       |                       | Symbol that           |
        |                       |                       | represents recursive  |
        |                       |                       | pattern               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ROOT_SYMBOL`         | ::: block             |
        |                       |                       | Delimiter that splits |
        |                       |                       | cell name and the     |
        |                       |                       | rest of the pattern   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static char`         | `TARGET_SYMBOL`       | ::: block             |
        |                       |                       | Delimiter that splits |
        |                       |                       | target name and the   |
        |                       |                       | rest of the pattern   |
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

        []{#ROOT_SYMBOL}

        -   #### ROOT_SYMBOL

                public static final String ROOT_SYMBOL

            ::: block
            Delimiter that splits cell name and the rest of the pattern
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants.ROOT_SYMBOL)

        []{#PATH_SYMBOL}

        -   #### PATH_SYMBOL

                public static final char PATH_SYMBOL

            ::: block
            Delimiter that splits path to a package root in the pattern
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants.PATH_SYMBOL)

        []{#TARGET_SYMBOL}

        -   #### TARGET_SYMBOL

                public static final char TARGET_SYMBOL

            ::: block
            Delimiter that splits target name and the rest of the
            pattern
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants.TARGET_SYMBOL)

        []{#RECURSIVE_SYMBOL}

        -   #### RECURSIVE_SYMBOL

                public static final String RECURSIVE_SYMBOL

            ::: block
            Symbol that represents recursive pattern
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants.RECURSIVE_SYMBOL)

        []{#FLAVOR_SYMBOL}

        -   #### FLAVOR_SYMBOL

                public static final char FLAVOR_SYMBOL

            ::: block
            Symbol that represents flavor part of a build target
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants.FLAVOR_SYMBOL)

        []{#FLAVOR_DELIMITER}

        -   #### FLAVOR_DELIMITER

                public static final char FLAVOR_DELIMITER

            ::: block
            Symbol that delimits flavors specified after FLAVOR_SYMBOL
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.parser.buildtargetpattern.BuildTargetLanguageConstants.FLAVOR_DELIMITER)
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
