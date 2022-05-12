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
[Package]{.packageLabelInType} [com.facebook.buck.shell.programrunner](package-summary.html)
:::

## Interface ProgramRunner {#interface-programrunner .title title="Interface ProgramRunner"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DarwinSandboxProgramRunner`, `DirectProgramRunner`

    ------------------------------------------------------------------------

        public interface ProgramRunner

    ::: block
    Parameters that changes how a program is executed by changing its
    command line.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `enhanceCommandLin    | ::: block             |
        | ogle.common.collect.I | e​(com.google.common.c | Change program        |
        | mmutableList<String>` | ollect.ImmutableList< | command line with     |
        |                       | String> commandLine)` | arguments specific to |
        |                       |                       | these parameters.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `enhanceCom           | ::: block             |
        | ogle.common.collect.I | mandLineForDescriptio | Change program        |
        | mmutableList<String>` | n​(com.google.common.c | command line with     |
        |                       | ollect.ImmutableList< | arguments specific to |
        |                       | String> commandLine)` | these parameters.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `prepareForRun​(Proje  | ::: block             |
        |                       | ctFilesystem projectF | Initialization that   |
        |                       | ilesystem,            | needs to be performed |
        |                       |    Path programPath)` | before execution.     |
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

        []{#prepareForRun(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### prepareForRun

            ``` methodSignature
            void prepareForRun​(ProjectFilesystem projectFilesystem,
                               Path programPath)
                        throws IOException
            ```

            ::: block
            Initialization that needs to be performed before execution.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#enhanceCommandLine(com.google.common.collect.ImmutableList)}

        -   #### enhanceCommandLine

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> enhanceCommandLine​(com.google.common.collect.ImmutableList<String> commandLine)
            ```

            ::: block
            Change program command line with arguments specific to these
            parameters.
            :::

        []{#enhanceCommandLineForDescription(com.google.common.collect.ImmutableList)}

        -   #### enhanceCommandLineForDescription

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> enhanceCommandLineForDescription​(com.google.common.collect.ImmutableList<String> commandLine)
            ```

            ::: block
            Change program command line with arguments specific to these
            parameters. This is primarily used to construct new command
            line before
            [`prepareForRun(com.facebook.buck.io.filesystem.ProjectFilesystem, java.nio.file.Path)`](#prepareForRun(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path))
            was called.
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
