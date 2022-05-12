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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Interface FileAttributesScrubber {#interface-fileattributesscrubber .title title="Interface FileAttributesScrubber"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `FileScrubber`

    ------------------------------------------------------------------------

        public interface FileAttributesScrubber
        extends FileScrubber

    ::: block
    Created by beefon on 06/06/2016.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.io.file.FileScrubber}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.io.file.[FileScrubber](FileScrubber.html "interface in com.facebook.buck.io.file")

            `FileScrubber.ScrubException`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `scrubFil             | ::: block             |
        |                       | eWithPath​(Path path)` | Override this method  |
        |                       |                       | to perform the        |
        |                       |                       | modification of the   |
        |                       |                       | file attributes       |
        |                       |                       | (modification date,   |
        |                       |                       | creation date, etc.)  |
        |                       |                       | WARNING: You should   |
        |                       |                       | not delete, rename or |
        |                       |                       | move the file, as the |
        |                       |                       | the behaviour is      |
        |                       |                       | undefined.            |
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

        []{#scrubFileWithPath(java.nio.file.Path)}

        -   #### scrubFileWithPath

            ``` methodSignature
            void scrubFileWithPath​(Path path)
            ```

            ::: block
            Override this method to perform the modification of the file
            attributes (modification date, creation date, etc.) WARNING:
            You should not delete, rename or move the file, as the the
            behaviour is undefined.
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
-   [Nested](#nested.class.summary) \| 
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
