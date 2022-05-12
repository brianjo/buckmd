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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JUnitStep {#class-junitstep .title title="Class JUnitStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.jvm.java.JUnitStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class JUnitStep
        extends ShellStep
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Fields inherited from class com.facebook.buck.shell.[ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

            `workingDirectory`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JUnitStep​(ProjectFilesystem filesystem,          Map<String,​String> nativeLibsEnvironment,          Optional<Long> testRuleTimeoutMs,          Optional<Long> testCaseTimeoutMs,          com.google.common.collect.ImmutableMap<String,​String> env,          com.google.common.collect.ImmutableList<String> javaRuntimeLauncher,          com.facebook.buck.jvm.java.JUnitJvmArgs junitJvmArgs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `ensu                 | ::: block             |
        |                       | reClasspathArgfile()` | Ensures the classpath |
        |                       |                       | argfile for Java 9+   |
        |                       |                       | invocations has been  |
        |                       |                       | created.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `g                    | ::: block             |
        |                       | etClasspathArgfile()` | Returns the classpath |
        |                       |                       | argfile for Java 9+   |
        |                       |                       | invocations.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEnvir             | ::: block             |
        | ommon.collect.Immutab | onmentVariables​(Execu | Returns the           |
        | leMap<String,​String>` | tionContext context)` | environment variables |
        |                       |                       | to include when       |
        |                       |                       | running this          |
        |                       |                       | [`ShellStep`](        |
        |                       |                       | ../../shell/ShellStep |
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
        | `prot                 | `getTimeout()`        |                       |
        | ected Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Optio      | `ge                   |                       |
        | nal<java.util.functio | tTimeoutHandler​(Execu |                       |
        | n.Consumer<Process>>` | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasTimedOut()`       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

            `addOptions, getDescription, getDuration, getShellCommand, getShellCommandArgsForDescription, getStderr, getStdin, getStdout, shouldPrintStderr, shouldPrintStdout`

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Map,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,com.facebook.buck.jvm.java.JUnitJvmArgs)}

        -   #### JUnitStep

                public JUnitStep​(ProjectFilesystem filesystem,
                                 Map<String,​String> nativeLibsEnvironment,
                                 Optional<Long> testRuleTimeoutMs,
                                 Optional<Long> testCaseTimeoutMs,
                                 com.google.common.collect.ImmutableMap<String,​String> env,
                                 com.google.common.collect.ImmutableList<String> javaRuntimeLauncher,
                                 com.facebook.buck.jvm.java.JUnitJvmArgs junitJvmArgs)
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

        []{#getClasspathArgfile()}

        -   #### getClasspathArgfile

            ``` methodSignature
            public Path getClasspathArgfile()
            ```

            ::: block
            Returns the classpath argfile for Java 9+ invocations.
            :::

        []{#ensureClasspathArgfile()}

        -   #### ensureClasspathArgfile

            ``` methodSignature
            public void ensureClasspathArgfile()
                                        throws IOException
            ```

            ::: block
            Ensures the classpath argfile for Java 9+ invocations has
            been created.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

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

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws InterruptedException,
                                               IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Overrides:]{.overrideSpecifyLabel}
            :   `execute` in class `ShellStep`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

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
            [`ShellStep`](../../shell/ShellStep.html "class in com.facebook.buck.shell").
            By default, this method returns an empty map.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getEnvironmentVariables` in class `ShellStep`

            [Parameters:]{.paramLabel}
            :   `context` - that may be useful when determining
                environment variables to include.

        []{#getTimeout()}

        -   #### getTimeout

            ``` methodSignature
            protected Optional<Long> getTimeout()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getTimeout` in class `ShellStep`

            [Returns:]{.returnLabel}
            :   an optional timeout to apply to the step.

        []{#getTimeoutHandler(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getTimeoutHandler

            ``` methodSignature
            protected Optional<java.util.function.Consumer<Process>> getTimeoutHandler​(ExecutionContext context)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getTimeoutHandler` in class `ShellStep`

            [Returns:]{.returnLabel}
            :   an optional timeout handler `Function` to do something
                before the process is killed.

        []{#getExitCodeFromResult(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.util.ProcessExecutor.Result)}

        -   #### getExitCodeFromResult

            ``` methodSignature
            protected int getExitCodeFromResult​(ExecutionContext context,
                                                ProcessExecutor.Result result)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getExitCodeFromResult` in class `ShellStep`

            [Returns:]{.returnLabel}
            :   the exit code interpreted from the `result`.

        []{#hasTimedOut()}

        -   #### hasTimedOut

            ``` methodSignature
            public boolean hasTimedOut()
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
