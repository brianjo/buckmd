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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.classes](package-summary.html)
:::

## Interface FileLike {#interface-filelike .title title="Interface FileLike"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractFileLike`

    ------------------------------------------------------------------------

        public interface FileLike

    ::: block
    Provides a file-like interface for objects which may be present
    within more specialized containers (like zip files).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getContainer()`      | ::: block             |
        |                       |                       | Returns the           |
        |                       |                       | containing file for   |
        |                       |                       | this file-like entry. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getInput()`          | ::: block             |
        |                       |                       | Opens a new input     |
        |                       |                       | stream for the entry. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRelativePath()`   | ::: block             |
        |                       |                       | Returns the relative  |
        |                       |                       | path for the entry.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getSize()`           | ::: block             |
        |                       |                       | Returns the size of   |
        |                       |                       | the entry in bytes.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getContainer()}

        -   #### getContainer

            ``` methodSignature
            Path getContainer()
            ```

            ::: block
            Returns the containing file for this file-like entry.
            :::

        []{#getRelativePath()}

        -   #### getRelativePath

            ``` methodSignature
            String getRelativePath()
            ```

            ::: block
            Returns the relative path for the entry. For example, if
            this were a zip file, this would be the relative path of a
            particular item in the zip file.
            :::

        []{#getSize()}

        -   #### getSize

            ``` methodSignature
            long getSize()
                  throws IOException
            ```

            ::: block
            Returns the size of the entry in bytes.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getInput()}

        -   #### getInput

            ``` methodSignature
            InputStream getInput()
                          throws IOException
            ```

            ::: block
            Opens a new input stream for the entry. This can be repeated
            to open the file-like object multiple times.
            :::

            [Returns:]{.returnLabel}
            :   Newly opened input stream.

            [Throws:]{.throwsLabel}
            :   `IOException` - An error occurred opening the stream.
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
