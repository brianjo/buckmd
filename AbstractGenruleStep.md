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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class AbstractGenruleStep {#class-abstractgenrulestep .title title="Class AbstractGenruleStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.shell.AbstractGenruleStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public abstract class AbstractGenruleStep
        extends ShellStep
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                 Description
          ------------------- ------------------------------------- -------------
          `static class `     `AbstractGenruleStep.CommandString`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Fields inherited from class com.facebook.buck.shell.[ShellStep](ShellStep.html "class in com.facebook.buck.shell")

            `workingDirectory`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AbstractGenruleStep​(ProjectFilesystem projectFilesystem,                    AbstractGenruleStep.CommandString commandString,                    AbsPath workingDirectory)`                                                 
          `AbstractGenruleStep​(ProjectFilesystem projectFilesystem,                    AbstractGenruleStep.CommandString commandString,                    Path workingDirectory)`                                                    
          `AbstractGenruleStep​(ProjectFilesystem projectFilesystem,                    AbstractGenruleStep.CommandString commandString,                    Path workingDirectory,                    ProgramRunner programRunner)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `addEnvironmentVar    |                       |
        | tected abstract void` | iables​(ExecutionConte |                       |
        |                       | xt context,           |                       |
        |                       |               com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableMap.Builder<St |                       |
        |                       | ring,​String> environm |                       |
        |                       | entVariablesBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
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
        | `String`              | `getScr               |                       |
        |                       | iptFileContents​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `ge                   |                       |
        |                       | tScriptFilePath​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.go     | `getShellCommandArg   |                       |
        | ogle.common.collect.I | sForDescription​(Execu |                       |
        | mmutableList<String>` | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.go     | `getShell             | ::: block             |
        | ogle.common.collect.I | CommandInternal​(Execu | Implementations of    |
        | mmutableList<String>` | tionContext context)` | this method should    |
        |                       |                       | not have any          |
        |                       |                       | observable            |
        |                       |                       | side-effects.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `shouldPrintStderr​(   |                       |
        |                       | Verbosity verbosity)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](ShellStep.html "class in com.facebook.buck.shell")

            `addOptions, getDescription, getDuration, getExitCodeFromResult, getShellCommand, getStderr, getStdin, getStdout, getTimeout, getTimeoutHandler, shouldPrintStdout`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.shell.AbstractGenruleStep.CommandString,java.nio.file.Path,com.facebook.buck.shell.programrunner.ProgramRunner)}

        -   #### AbstractGenruleStep

                public AbstractGenruleStep​(ProjectFilesystem projectFilesystem,
                                           AbstractGenruleStep.CommandString commandString,
                                           Path workingDirectory,
                                           ProgramRunner programRunner)

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.shell.AbstractGenruleStep.CommandString,java.nio.file.Path)}

        -   #### AbstractGenruleStep

                public AbstractGenruleStep​(ProjectFilesystem projectFilesystem,
                                           AbstractGenruleStep.CommandString commandString,
                                           Path workingDirectory)

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.shell.AbstractGenruleStep.CommandString,com.facebook.buck.core.filesystems.AbsPath)}

        -   #### AbstractGenruleStep

                public AbstractGenruleStep​(ProjectFilesystem projectFilesystem,
                                           AbstractGenruleStep.CommandString commandString,
                                           AbsPath workingDirectory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException,
                                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Overrides:]{.overrideSpecifyLabel}
            :   `execute` in class `ShellStep`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getShellCommandInternal(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getShellCommandInternal

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getShellCommandInternal​(ExecutionContext context)
            ```

            ::: block
            [Description copied from
            class: `ShellStep`]{.descfrmTypeLabel}
            :::

            ::: block
            Implementations of this method should not have any
            observable side-effects.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShellCommandInternal` in class `ShellStep`

        []{#getShellCommandArgsForDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getShellCommandArgsForDescription

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getShellCommandArgsForDescription​(ExecutionContext context)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getShellCommandArgsForDescription` in class `ShellStep`

        []{#getEnvironmentVariables(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getEnvironmentVariables

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironmentVariables​(ExecutionContext context)
            ```

            ::: block
            [Description copied from
            class: `ShellStep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the environment variables to include when running
            this
            [`ShellStep`](ShellStep.html "class in com.facebook.buck.shell").
            By default, this method returns an empty map.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getEnvironmentVariables` in class `ShellStep`

            [Parameters:]{.paramLabel}
            :   `context` - that may be useful when determining
                environment variables to include.

        []{#shouldPrintStderr(com.facebook.buck.util.Verbosity)}

        -   #### shouldPrintStderr

            ``` methodSignature
            protected boolean shouldPrintStderr​(Verbosity verbosity)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldPrintStderr` in class `ShellStep`

            [Returns:]{.returnLabel}
            :   whether the stderr of the shell command, when executed,
                should be printed to the stderr of the specified
                [`ExecutionContext`](../core/build/execution/context/ExecutionContext.html "class in com.facebook.buck.core.build.execution.context").
                If `false`, stderr will only be printed on error and
                only if verbosity is set to standard information.

        []{#getScriptFileContents(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getScriptFileContents

            ``` methodSignature
            public String getScriptFileContents​(ExecutionContext context)
            ```

        []{#getScriptFilePath(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getScriptFilePath

            ``` methodSignature
            public Path getScriptFilePath​(ExecutionContext context)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#addEnvironmentVariables(com.facebook.buck.core.build.execution.context.ExecutionContext,com.google.common.collect.ImmutableMap.Builder)}

        -   #### addEnvironmentVariables

            ``` methodSignature
            protected abstract void addEnvironmentVariables​(ExecutionContext context,
                                                            com.google.common.collect.ImmutableMap.Builder<String,​String> environmentVariablesBuilder)
            ```
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
