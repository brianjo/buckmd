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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Class GoListStep {#class-goliststep .title title="Class GoListStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.features.go.GoListStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class GoListStep
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

          Constructor                                                                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GoListStep​(Path workingDirectory,           Optional<Path> targetFile,           com.facebook.buck.features.go.GoPlatform platform,           List<com.facebook.buck.features.go.GoListStep.ListType> listTypes)`    

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
        | `String`              | `getRawOutput()`      |                       |
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
        | `Set<Path>`           | `getSourceFiles()`    |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

            `execute, getDescription, getDuration, getExitCodeFromResult, getShellCommand, getShellCommandArgsForDescription, getStderr, getStdin, getStdout, getTimeout, getTimeoutHandler, shouldPrintStderr, shouldPrintStdout`

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

        []{#<init>(java.nio.file.Path,java.util.Optional,com.facebook.buck.features.go.GoPlatform,java.util.List)}

        -   #### GoListStep

                public GoListStep​(Path workingDirectory,
                                  Optional<Path> targetFile,
                                  com.facebook.buck.features.go.GoPlatform platform,
                                  List<com.facebook.buck.features.go.GoListStep.ListType> listTypes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#addOptions(com.google.common.collect.ImmutableSet.Builder)}

        -   #### addOptions

            ``` methodSignature
            protected void addOptions​(com.google.common.collect.ImmutableSet.Builder<ProcessExecutor.Option> options)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `addOptions` in class `ShellStep`

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

        []{#getRawOutput()}

        -   #### getRawOutput

            ``` methodSignature
            public String getRawOutput()
            ```

        []{#getSourceFiles()}

        -   #### getSourceFiles

            ``` methodSignature
            public Set<Path> getSourceFiles()
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