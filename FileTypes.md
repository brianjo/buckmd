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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode.xcodeproj](package-summary.html)
:::

## Class FileTypes {#class-filetypes .title title="Class FileTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.xcode.xcodeproj.FileTypes

::: description
-   

    ------------------------------------------------------------------------

        public final class FileTypes
        extends Object

    ::: block
    File types used in Apple targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static com.g         | `EXPLICIT_FILE_TYP    | ::: block             |
        | oogle.common.collect. | E_BROKEN_IDENTIFIERS` | Set of identifiers    |
        | ImmutableSet<String>` |                       | which only work as    |
        |                       |                       | \"lastKnownFileType\" |
        |                       |                       | and not               |
        |                       |                       | \"explicitFileType\"  |
        |                       |                       | in a                  |
        |                       |                       | PBXFileReference.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `FILE_EXT             | ::: block             |
        | ommon.collect.Immutab | ENSION_TO_IDENTIFIER` | Map of file extension |
        | leMap<String,​String>` |                       | to Xcode identifiers. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `MODIFIABLE_F         | ::: block             |
        | oogle.common.collect. | ILE_TYPE_IDENTIFIERS` | Set of identifiers    |
        | ImmutableSet<String>` |                       | for which we will use |
        |                       |                       | \"lastKnownFileType\" |
        |                       |                       | instead of            |
        |                       |                       | \"explicitFileType\"  |
        |                       |                       | in a PBXFileReference |
        |                       |                       | to allow the user to  |
        |                       |                       | change the type by    |
        |                       |                       | renaming the file.    |
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

        []{#FILE_EXTENSION_TO_IDENTIFIER}

        -   #### FILE_EXTENSION_TO_IDENTIFIER

                public static final com.google.common.collect.ImmutableMap<String,​String> FILE_EXTENSION_TO_IDENTIFIER

            ::: block
            Map of file extension to Xcode identifiers.
            :::

        []{#EXPLICIT_FILE_TYPE_BROKEN_IDENTIFIERS}

        -   #### EXPLICIT_FILE_TYPE_BROKEN_IDENTIFIERS

                public static final com.google.common.collect.ImmutableSet<String> EXPLICIT_FILE_TYPE_BROKEN_IDENTIFIERS

            ::: block
            Set of identifiers which only work as \"lastKnownFileType\"
            and not \"explicitFileType\" in a PBXFileReference.
            Yes, really. Because Xcode.
            :::

        []{#MODIFIABLE_FILE_TYPE_IDENTIFIERS}

        -   #### MODIFIABLE_FILE_TYPE_IDENTIFIERS

                public static final com.google.common.collect.ImmutableSet<String> MODIFIABLE_FILE_TYPE_IDENTIFIERS

            ::: block
            Set of identifiers for which we will use
            \"lastKnownFileType\" instead of \"explicitFileType\" in a
            PBXFileReference to allow the user to change the type by
            renaming the file.
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
