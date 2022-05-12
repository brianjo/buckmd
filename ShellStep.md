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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class ShellStep {#class-shellstep .title title="Class ShellStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.ShellStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AaptStep`, `AbstractGenruleStep`, `AidlStep`, `BashStep`,
        `CGoCompileStep`, `CGoGenerateImportStep`,
        `CsharpLibraryCompile`, `DCompileStep`, `DefaultShellStep`,
        `DxStep`, `GenerateCodeCoverageReportStep`, `GoAssembleStep`,
        `GoCompileStep`, `GoLinkStep`, `GoListStep`, `GoPackStep`,
        `GoTestCoverStep`, `GoTestMainStep`, `HalideCompilerStep`,
        `InstrumentationStep`, `JUnitStep`, `LibtoolStep`,
        `MachoScrubContentSectionsStep`, `NdkBuildStep`,
        `OcamlCCompileStep`, `OcamlDepToolStep`, `OcamlLexStep`,
        `OcamlLinkStep`, `OcamlMLCompileStep`, `OcamlNativePluginStep`,
        `OcamlYaccStep`, `PexStep`, `ProGuardObfuscateStep`,
        `ReDexStep`, `ScalacStep`, `StripStep`, `ZipalignStep`

    ------------------------------------------------------------------------

        public abstract class ShellStep
        extends Object
        implements Step
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `protected Path`      | `workingDirectory`    | ::: block             |
        |                       |                       | If specified, working |
        |                       |                       | directory will be     |
        |                       |                       | different from build  |
        |                       |                       | cell root.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                             Description
          -------------- --------------------------------------- -------------
          `protected `   `ShellStep​(AbsPath workingDirectory)`    
          `protected `   `ShellStep​(Path workingDirectory)`       

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `addOpti              |                       |
        |                       | ons​(com.google.common |                       |
        |                       | .collect.ImmutableSet |                       |
        |                       | .Builder<ProcessExecu |                       |
        |                       | tor.Option> options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDescription​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getDuration()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEnvir             | ::: block             |
        | ommon.collect.Immutab | onmentVariables​(Execu | Returns the           |
        | leMap<String,​String>` | tionContext context)` | environment variables |
        |                       |                       | to include when       |
        |                       |                       | running this          |
        |                       |                       | [`                    |
        |                       |                       | ShellStep`](ShellStep |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.shell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected int`       | `getExitCodeFromR     |                       |
        |                       | esult​(ExecutionContex |                       |
        |                       | t context,            |                       |
        |                       |            ProcessExe |                       |
        |                       | cutor.Result result)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     | ::: block             |
        | ogle.common.collect.I | getShellCommand​(Execu | This method is        |
        | mmutableList<String>` | tionContext context)` | idempotent.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.go     | `getShellCommandArg   |                       |
        | ogle.common.collect.I | sForDescription​(Execu |                       |
        | mmutableList<String>` | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `getShell             | ::: block             |
        | ected abstract com.go | CommandInternal​(Execu | Implementations of    |
        | ogle.common.collect.I | tionContext context)` | this method should    |
        | mmutableList<String>` |                       | not have any          |
        |                       |                       | observable            |
        |                       |                       | side-effects.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStderr()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getStdin​(Execu       |                       |
        | ted Optional<String>` | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStdout()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `getTimeout()`        |                       |
        | ected Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Optio      | `ge                   |                       |
        | nal<java.util.functio | tTimeoutHandler​(Execu |                       |
        | n.Consumer<Process>>` | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `shouldPrintStderr​(   |                       |
        |                       | Verbosity verbosity)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `shouldPrintStdout​(   |                       |
        |                       | Verbosity verbosity)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.step.Step}

            ### Methods inherited from interface com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step")

            `getShortName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#workingDirectory}

        -   #### workingDirectory

                protected final Path workingDirectory

            ::: block
            If specified, working directory will be different from build
            cell root. This should be relative to the build cell root.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path)}

        -   #### ShellStep

                protected ShellStep​(Path workingDirectory)

        []{#<init>(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### ShellStep

                protected ShellStep​(AbsPath workingDirectory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws InterruptedException,
                                               IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#getExitCodeFromResult(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.util.ProcessExecutor.Result)}

        -   #### getExitCodeFromResult

            ``` methodSignature
            protected int getExitCodeFromResult​(ExecutionContext context,
                                                ProcessExecutor.Result result)
            ```

            [Returns:]{.returnLabel}
            :   the exit code interpreted from the `result`.

        []{#addOptions(com.google.common.collect.ImmutableSet.Builder)}

        -   #### addOptions

            ``` methodSignature
            protected void addOptions​(com.google.common.collect.ImmutableSet.Builder<ProcessExecutor.Option> options)
            ```

        []{#getDuration()}

        -   #### getDuration

            ``` methodSignature
            public long getDuration()
            ```

        []{#getShellCommand(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getShellCommand

            ``` methodSignature
            public final com.google.common.collect.ImmutableList<String> getShellCommand​(ExecutionContext context)
            ```

            ::: block
            This method is idempotent.
            :::

            [Returns:]{.returnLabel}
            :   the shell command arguments

        []{#getShellCommandArgsForDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getShellCommandArgsForDescription

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getShellCommandArgsForDescription​(ExecutionContext context)
            ```

        []{#getStdin(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getStdin

            ``` methodSignature
            protected Optional<String> getStdin​(ExecutionContext context)
                                         throws InterruptedException,
                                                IOException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#getShellCommandInternal(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getShellCommandInternal

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableList<String> getShellCommandInternal​(ExecutionContext context)
            ```

            ::: block
            Implementations of this method should not have any
            observable side-effects.
            :::

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public final String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`

        []{#getEnvironmentVariables(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getEnvironmentVariables

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironmentVariables​(ExecutionContext context)
            ```

            ::: block
            Returns the environment variables to include when running
            this
            [`ShellStep`](ShellStep.html "class in com.facebook.buck.shell").
            By default, this method returns an empty map.
            :::

            [Parameters:]{.paramLabel}
            :   `context` - that may be useful when determining
                environment variables to include.

        []{#shouldPrintStdout(com.facebook.buck.util.Verbosity)}

        -   #### shouldPrintStdout

            ``` methodSignature
            protected boolean shouldPrintStdout​(Verbosity verbosity)
            ```

            [Parameters:]{.paramLabel}
            :   `verbosity` - is provided in case that affects what
                should be printed.

            [Returns:]{.returnLabel}
            :   whether the stdout of the shell command, when executed,
                should be printed to the stderr of the specified
                [`ExecutionContext`](../core/build/execution/context/ExecutionContext.html "class in com.facebook.buck.core.build.execution.context").
                If `false`, stdout will only be printed on error and
                only if verbosity is set to standard information.

        []{#getStdout()}

        -   #### getStdout

            ``` methodSignature
            public final String getStdout()
            ```

            [Returns:]{.returnLabel}
            :   the stdout of this ShellCommand or throws an exception
                if the stdout was not recorded

        []{#shouldPrintStderr(com.facebook.buck.util.Verbosity)}

        -   #### shouldPrintStderr

            ``` methodSignature
            protected boolean shouldPrintStderr​(Verbosity verbosity)
            ```

            [Returns:]{.returnLabel}
            :   whether the stderr of the shell command, when executed,
                should be printed to the stderr of the specified
                [`ExecutionContext`](../core/build/execution/context/ExecutionContext.html "class in com.facebook.buck.core.build.execution.context").
                If `false`, stderr will only be printed on error and
                only if verbosity is set to standard information.

        []{#getStderr()}

        -   #### getStderr

            ``` methodSignature
            public final String getStderr()
            ```

            [Returns:]{.returnLabel}
            :   the stderr of this ShellCommand or throws an exception
                if the stderr was not recorded

        []{#getTimeout()}

        -   #### getTimeout

            ``` methodSignature
            protected Optional<Long> getTimeout()
            ```

            [Returns:]{.returnLabel}
            :   an optional timeout to apply to the step.

        []{#getTimeoutHandler(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getTimeoutHandler

            ``` methodSignature
            protected Optional<java.util.function.Consumer<Process>> getTimeoutHandler​(ExecutionContext context)
            ```

            [Returns:]{.returnLabel}
            :   an optional timeout handler `Function` to do something
                before the process is killed.
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
