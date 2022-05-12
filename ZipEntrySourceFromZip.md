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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip.collect](package-summary.html)
:::

## Interface ZipEntrySourceFromZip {#interface-zipentrysourcefromzip .title title="Interface ZipEntrySourceFromZip"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ZipEntrySource`

    ------------------------------------------------------------------------

        public interface ZipEntrySourceFromZip
        extends ZipEntrySource

    ::: block
    A source for a zip file entry that represents an entry for another
    zip file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getEntryName()`      | ::: block             |
        |                       |                       | The name of the entry |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getEntryPosition()`  | ::: block             |
        |                       |                       | Position of the entry |
        |                       |                       | in the list of        |
        |                       |                       | entries.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getSourceFilePath()` | ::: block             |
        |                       |                       | Path to the source    |
        |                       |                       | zip file.             |
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

        []{#getSourceFilePath()}

        -   #### getSourceFilePath

            ``` methodSignature
            Path getSourceFilePath()
            ```

            ::: block
            Path to the source zip file.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourceFilePath` in interface `ZipEntrySource`

        []{#getEntryName()}

        -   #### getEntryName

            ``` methodSignature
            String getEntryName()
            ```

            ::: block
            The name of the entry
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEntryName` in interface `ZipEntrySource`

        []{#getEntryPosition()}

        -   #### getEntryPosition

            ``` methodSignature
            int getEntryPosition()
            ```

            ::: block
            Position of the entry in the list of entries.
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
