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
[Package]{.packageLabelInType} [com.facebook.buck.sandbox.darwin](package-summary.html)
:::

## Class DarwinSandboxProgramRunner {#class-darwinsandboxprogramrunner .title title="Class DarwinSandboxProgramRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.sandbox.darwin.DarwinSandboxProgramRunner

::: description
-   

    All Implemented Interfaces:
    :   `ProgramRunner`

    ------------------------------------------------------------------------

        public class DarwinSandboxProgramRunner
        extends Object
        implements ProgramRunner

    ::: block
    [`ProgramRunner`](../../shell/programrunner/ProgramRunner.html "interface in com.facebook.buck.shell.programrunner")
    that runs a program in an OS X sandbox.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                         Description
          ------------------------------------------------------------------- -------------
          `DarwinSandboxProgramRunner​(SandboxProperties sandboxProperties)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.sandbox.SandboxProperties)}

        -   #### DarwinSandboxProgramRunner

                public DarwinSandboxProgramRunner​(SandboxProperties sandboxProperties)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#prepareForRun(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### prepareForRun

            ``` methodSignature
            public void prepareForRun​(ProjectFilesystem projectFilesystem,
                                      Path programPath)
                               throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProgramRunner`]{.descfrmTypeLabel}
            :::

            ::: block
            Initialization that needs to be performed before execution.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `prepareForRun` in interface `ProgramRunner`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#enhanceCommandLine(com.google.common.collect.ImmutableList)}

        -   #### enhanceCommandLine

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> enhanceCommandLine​(com.google.common.collect.ImmutableList<String> commandLine)
            ```

            ::: block
            [Description copied from
            interface: `ProgramRunner`]{.descfrmTypeLabel}
            :::

            ::: block
            Change program command line with arguments specific to these
            parameters.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `enhanceCommandLine` in interface `ProgramRunner`

        []{#enhanceCommandLineForDescription(com.google.common.collect.ImmutableList)}

        -   #### enhanceCommandLineForDescription

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> enhanceCommandLineForDescription​(com.google.common.collect.ImmutableList<String> commandLine)
            ```

            ::: block
            [Description copied from
            interface: `ProgramRunner`]{.descfrmTypeLabel}
            :::

            ::: block
            Change program command line with arguments specific to these
            parameters. This is primarily used to construct new command
            line before
            [`ProgramRunner.prepareForRun(com.facebook.buck.io.filesystem.ProjectFilesystem, java.nio.file.Path)`](../../shell/programrunner/ProgramRunner.html#prepareForRun(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path))
            was called.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `enhanceCommandLineForDescription` in
                interface `ProgramRunner`
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
