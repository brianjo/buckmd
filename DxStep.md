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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class DxStep {#class-dxstep .title title="Class DxStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.android.DxStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class DxStep
        extends ShellStep
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `DxStep.Option`       | ::: block             |
        |                       |                       | Options to pass to    |
        |                       |                       | `dx`.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `D8`                  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEX_REFERENC         |                       |
        |                       | E_OVERFLOW_EXIT_CODE` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `DX`                  | ::: block             |
        |                       |                       | Available tools to    |
        |                       |                       | create dex files \*   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `FAILURE_EXIT_CODE`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `SUCCESS_EXIT_CODE`   |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Fields inherited from class com.facebook.buck.shell.[ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

            `workingDirectory`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DxStep​(ProjectFilesystem filesystem,       AndroidPlatformTarget androidPlatformTarget,       Path outputDexFile,       Iterable<Path> filesToDex)`                                                                                                                                                                                                                                               
          `DxStep​(ProjectFilesystem filesystem,       AndroidPlatformTarget androidPlatformTarget,       Path outputDexFile,       Iterable<Path> filesToDex,       EnumSet<DxStep.Option> options,       String dexTool)`                                                                                                                                                                                   
          `DxStep​(ProjectFilesystem filesystem,       AndroidPlatformTarget androidPlatformTarget,       Path outputDexFile,       Iterable<Path> filesToDex,       EnumSet<DxStep.Option> options,       Optional<String> maxHeapSize,       String dexTool,       boolean intermediate)`                                                                                                                   
          `DxStep​(ProjectFilesystem filesystem,       AndroidPlatformTarget androidPlatformTarget,       Path outputDexFile,       Iterable<Path> filesToDex,       EnumSet<DxStep.Option> options,       Optional<String> maxHeapSize,       String dexTool,       boolean intermediate,       Collection<Path> classpathFiles,       Optional<String> bucketId,       Optional<Integer> minSdkVersion)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getOutputDexFile()`  |                       |
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
        | `protected boolean`   | `shouldPrintStdout​(   |                       |
        |                       | Verbosity verbosity)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

            `addOptions, getDescription, getDuration, getEnvironmentVariables, getExitCodeFromResult, getShellCommand, getShellCommandArgsForDescription, getStderr, getStdin, getStdout, getTimeout, getTimeoutHandler`

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
    -   []{#field.detail}

        ### Field Detail

        []{#SUCCESS_EXIT_CODE}

        -   #### SUCCESS_EXIT_CODE

                public static final int SUCCESS_EXIT_CODE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.DxStep.SUCCESS_EXIT_CODE)

        []{#FAILURE_EXIT_CODE}

        -   #### FAILURE_EXIT_CODE

                public static final int FAILURE_EXIT_CODE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.DxStep.FAILURE_EXIT_CODE)

        []{#DEX_REFERENCE_OVERFLOW_EXIT_CODE}

        -   #### DEX_REFERENCE_OVERFLOW_EXIT_CODE

                public static final int DEX_REFERENCE_OVERFLOW_EXIT_CODE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.DxStep.DEX_REFERENCE_OVERFLOW_EXIT_CODE)

        []{#DX}

        -   #### DX

                public static final String DX

            ::: block
            Available tools to create dex files \*
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.DxStep.DX)

        []{#D8}

        -   #### D8

                public static final String D8

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.DxStep.D8)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.android.toolchain.AndroidPlatformTarget,java.nio.file.Path,java.lang.Iterable)}

        -   #### DxStep

                public DxStep​(ProjectFilesystem filesystem,
                              AndroidPlatformTarget androidPlatformTarget,
                              Path outputDexFile,
                              Iterable<Path> filesToDex)

            [Parameters:]{.paramLabel}
            :   `outputDexFile` - path to the file where the generated
                classes.dex should go.
            :   `filesToDex` - each element in this set is a path to a
                .class file, a zip file of .class files, or a directory
                of .class files.

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.android.toolchain.AndroidPlatformTarget,java.nio.file.Path,java.lang.Iterable,java.util.EnumSet,java.lang.String)}

        -   #### DxStep

                public DxStep​(ProjectFilesystem filesystem,
                              AndroidPlatformTarget androidPlatformTarget,
                              Path outputDexFile,
                              Iterable<Path> filesToDex,
                              EnumSet<DxStep.Option> options,
                              String dexTool)

            [Parameters:]{.paramLabel}
            :   `outputDexFile` - path to the file where the generated
                classes.dex should go.
            :   `filesToDex` - each element in this set is a path to a
                .class file, a zip file of .class files, or a directory
                of .class files.
            :   `options` - to pass to `dx`.
            :   `dexTool` - the tool used to perform dexing.

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.android.toolchain.AndroidPlatformTarget,java.nio.file.Path,java.lang.Iterable,java.util.EnumSet,java.util.Optional,java.lang.String,boolean)}

        -   #### DxStep

                public DxStep​(ProjectFilesystem filesystem,
                              AndroidPlatformTarget androidPlatformTarget,
                              Path outputDexFile,
                              Iterable<Path> filesToDex,
                              EnumSet<DxStep.Option> options,
                              Optional<String> maxHeapSize,
                              String dexTool,
                              boolean intermediate)

            [Parameters:]{.paramLabel}
            :   `outputDexFile` - path to the file where the generated
                classes.dex should go.
            :   `filesToDex` - each element in this set is a path to a
                .class file, a zip file of .class files, or a directory
                of .class files.
            :   `options` - to pass to `dx`.
            :   `maxHeapSize` - The max heap size used for out of
                process dex.
            :   `dexTool` - the tool used to perform dexing.

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.android.toolchain.AndroidPlatformTarget,java.nio.file.Path,java.lang.Iterable,java.util.EnumSet,java.util.Optional,java.lang.String,boolean,java.util.Collection,java.util.Optional,java.util.Optional)}

        -   #### DxStep

                public DxStep​(ProjectFilesystem filesystem,
                              AndroidPlatformTarget androidPlatformTarget,
                              Path outputDexFile,
                              Iterable<Path> filesToDex,
                              EnumSet<DxStep.Option> options,
                              Optional<String> maxHeapSize,
                              String dexTool,
                              boolean intermediate,
                              @Nullable
                              Collection<Path> classpathFiles,
                              Optional<String> bucketId,
                              Optional<Integer> minSdkVersion)

            [Parameters:]{.paramLabel}
            :   `outputDexFile` - path to the file where the generated
                classes.dex should go.
            :   `filesToDex` - each element in this set is a path to a
                .class file, a zip file of .class files, or a directory
                of .class files.
            :   `options` - to pass to `dx`.
            :   `maxHeapSize` - The max heap size used for out of
                process dex.
            :   `dexTool` - the tool used to perform dexing.
            :   `classpathFiles` - specifies classpath for interface
                static and default methods desugaring.
            :   `minSdkVersion` -
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

        []{#shouldPrintStdout(com.facebook.buck.util.Verbosity)}

        -   #### shouldPrintStdout

            ``` methodSignature
            protected boolean shouldPrintStdout​(Verbosity verbosity)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shouldPrintStdout` in class `ShellStep`

            [Parameters:]{.paramLabel}
            :   `verbosity` - is provided in case that affects what
                should be printed.

            [Returns:]{.returnLabel}
            :   whether the stdout of the shell command, when executed,
                should be printed to the stderr of the specified
                [`ExecutionContext`](../core/build/execution/context/ExecutionContext.html "class in com.facebook.buck.core.build.execution.context").
                If `false`, stdout will only be printed on error and
                only if verbosity is set to standard information.

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getOutputDexFile()}

        -   #### getOutputDexFile

            ``` methodSignature
            public Path getOutputDexFile()
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
