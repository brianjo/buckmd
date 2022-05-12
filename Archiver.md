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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface Archiver {#interface-archiver .title title="Interface Archiver"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Tool`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BsdArchiver`, `ClangWindowsArchiver`, `GnuArchiver`,
        `WindowsArchiver`

    ------------------------------------------------------------------------

        public interface Archiver
        extends Tool

    ::: block
    Interface for a c/c++ archiver.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `getArchiveOptions​(bo |                       |
        | ogle.common.collect.I | olean isThinArchive)` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getScrubbers()`      |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<FileScrubber>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isArgfileRequired()` | ::: block             |
        |                       |                       | Whether an argfile is |
        |                       |                       | required for a long   |
        |                       |                       | command line (false   |
        |                       |                       | means that it is      |
        |                       |                       | possible to split a   |
        |                       |                       | long command line     |
        |                       |                       | into chunks).         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `is                   |                       |
        |                       | RanLibStepRequired()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `outputArg            |                       |
        | ogle.common.collect.I | s​(String outputPath)` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `su                   |                       |
        |                       | pportsThinArchives()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScrubbers()}

        -   #### getScrubbers

            ``` methodSignature
            com.google.common.collect.ImmutableList<FileScrubber> getScrubbers()
            ```

        []{#supportsThinArchives()}

        -   #### supportsThinArchives

            ``` methodSignature
            boolean supportsThinArchives()
            ```

        []{#getArchiveOptions(boolean)}

        -   #### getArchiveOptions

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getArchiveOptions​(boolean isThinArchive)
            ```

        []{#outputArgs(java.lang.String)}

        -   #### outputArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> outputArgs​(String outputPath)
            ```

        []{#isRanLibStepRequired()}

        -   #### isRanLibStepRequired

            ``` methodSignature
            boolean isRanLibStepRequired()
            ```

        []{#isArgfileRequired()}

        -   #### isArgfileRequired

            ``` methodSignature
            boolean isArgfileRequired()
            ```

            ::: block
            Whether an argfile is required for a long command line
            (false means that it is possible to split a long command
            line into chunks). Eg, ar on \*nix allows to add new files
            to an already created archive, but doesn\'t accept argfiles.
            On the contrary, VS lib.exe on windows always overrides the
            previous archive, but supports argfiles.
            :::

            [Returns:]{.returnLabel}
            :   whether \@argfile is required for a long command line
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
