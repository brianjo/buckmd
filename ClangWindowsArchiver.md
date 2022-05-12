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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class ClangWindowsArchiver {#class-clangwindowsarchiver .title title="Class ClangWindowsArchiver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.tool.DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

    -   -   com.facebook.buck.cxx.toolchain.ClangWindowsArchiver

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Archiver`

    ------------------------------------------------------------------------

        public class ClangWindowsArchiver
        extends DelegatingTool
        implements Archiver

    ::: block
    Archiver implementation for the Clang for Windows toolchain.
    The implementation currently is only suitable for generating .lib
    archives for Windows-targeted builds, for ingestion by either
    link.exe or lld-link.exe. If used with lld-link.exe, thin archives
    are an option. link.exe cannot ingest thin archives generated with
    this tool.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `ClangWindowsArchiver​(Tool tool)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.DelegatingTool}

            ### Methods inherited from class com.facebook.buck.core.toolchain.tool.[DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### ClangWindowsArchiver

                public ClangWindowsArchiver​(Tool tool)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScrubbers()}

        -   #### getScrubbers

            ``` methodSignature
            public com.google.common.collect.ImmutableList<FileScrubber> getScrubbers()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getScrubbers` in interface `Archiver`

        []{#supportsThinArchives()}

        -   #### supportsThinArchives

            ``` methodSignature
            public boolean supportsThinArchives()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsThinArchives` in interface `Archiver`

        []{#getArchiveOptions(boolean)}

        -   #### getArchiveOptions

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getArchiveOptions​(boolean isThinArchive)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getArchiveOptions` in interface `Archiver`

        []{#outputArgs(java.lang.String)}

        -   #### outputArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> outputArgs​(String outputPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `outputArgs` in interface `Archiver`

        []{#isRanLibStepRequired()}

        -   #### isRanLibStepRequired

            ``` methodSignature
            public boolean isRanLibStepRequired()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isRanLibStepRequired` in interface `Archiver`

        []{#isArgfileRequired()}

        -   #### isArgfileRequired

            ``` methodSignature
            public boolean isArgfileRequired()
            ```

            ::: block
            [Description copied from
            interface: `Archiver`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether an argfile is required for a long command line
            (false means that it is possible to split a long command
            line into chunks). Eg, ar on \*nix allows to add new files
            to an already created archive, but doesn\'t accept argfiles.
            On the contrary, VS lib.exe on windows always overrides the
            previous archive, but supports argfiles.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isArgfileRequired` in interface `Archiver`

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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
