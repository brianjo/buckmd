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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class ProGuardObfuscateStep {#class-proguardobfuscatestep .title title="Class ProGuardObfuscateStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.android.ProGuardObfuscateStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public final class ProGuardObfuscateStep
        extends ShellStep
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                           Description
          ------------------- ------------------------------- -------------
          `static int`        `DEFAULT_OPTIMIZATION_PASSES`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Fields inherited from class com.facebook.buck.shell.[ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

            `workingDirectory`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `create​(AndroidP      | ::: block             |
        |                       | latformTarget android | Create steps that     |
        |                       | PlatformTarget,       | write out ProGuard\'s |
        |                       |  com.google.common.co | command line          |
        |                       | llect.ImmutableList<S | arguments to a text   |
        |                       | tring> javaRuntimeLau | file and then run     |
        |                       | ncher,       ProjectF | ProGuard using those  |
        |                       | ilesystem filesystem, | arguments.            |
        |                       |        Optional<Path> | :::                   |
        |                       |  proguardJarOverride, |                       |
        |                       |        String proguar |                       |
        |                       | dMaxHeapSize,       O |                       |
        |                       | ptional<String> progu |                       |
        |                       | ardAgentPath,       S |                       |
        |                       | et<Path> customProgua |                       |
        |                       | rdConfigs,       com. |                       |
        |                       | facebook.buck.android |                       |
        |                       | .ProGuardObfuscateSte |                       |
        |                       | p.SdkProguardType sdk |                       |
        |                       | ProguardConfig,       |                       |
        |                       |  int optimizationPass |                       |
        |                       | es,       Optional<Li |                       |
        |                       | st<String>> proguardJ |                       |
        |                       | vmArgs,       Map<Pat |                       |
        |                       | h,​Path> inputAndOutpu |                       |
        |                       | tEntries,       com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableSet<Path> ad |                       |
        |                       | ditionalLibraryJarsFo |                       |
        |                       | rProguard,       Path |                       |
        |                       |  proguardDirectory,   |                       |
        |                       |      BuildableContext |                       |
        |                       |  buildableContext,    |                       |
        |                       |     BuildContext buil |                       |
        |                       | dContext,       boole |                       |
        |                       | an skipProguard,      |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<Step> steps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
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
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

            `addOptions, getDescription, getDuration, getEnvironmentVariables, getExitCodeFromResult, getShellCommand, getShellCommandArgsForDescription, getStderr, getStdin, getStdout, getTimeout, getTimeoutHandler, shouldPrintStderr, shouldPrintStdout`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_OPTIMIZATION_PASSES}

        -   #### DEFAULT_OPTIMIZATION_PASSES

                public static final int DEFAULT_OPTIMIZATION_PASSES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.ProGuardObfuscateStep.DEFAULT_OPTIMIZATION_PASSES)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.android.toolchain.AndroidPlatformTarget,com.google.common.collect.ImmutableList,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,java.lang.String,java.util.Optional,java.util.Set,com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType,int,java.util.Optional,java.util.Map,com.google.common.collect.ImmutableSet,java.nio.file.Path,com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.core.build.context.BuildContext,boolean,com.google.common.collect.ImmutableList.Builder)}

        -   #### create

            ``` methodSignature
            public static void create​(AndroidPlatformTarget androidPlatformTarget,
                                      com.google.common.collect.ImmutableList<String> javaRuntimeLauncher,
                                      ProjectFilesystem filesystem,
                                      Optional<Path> proguardJarOverride,
                                      String proguardMaxHeapSize,
                                      Optional<String> proguardAgentPath,
                                      Set<Path> customProguardConfigs,
                                      com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType sdkProguardConfig,
                                      int optimizationPasses,
                                      Optional<List<String>> proguardJvmArgs,
                                      Map<Path,​Path> inputAndOutputEntries,
                                      com.google.common.collect.ImmutableSet<Path> additionalLibraryJarsForProguard,
                                      Path proguardDirectory,
                                      BuildableContext buildableContext,
                                      BuildContext buildContext,
                                      boolean skipProguard,
                                      com.google.common.collect.ImmutableList.Builder<Step> steps)
            ```

            ::: block
            Create steps that write out ProGuard\'s command line
            arguments to a text file and then run ProGuard using those
            arguments. We write the arguments to a file to avoid blowing
            out exec()\'s ARG_MAX limit.
            :::

            [Parameters:]{.paramLabel}
            :   `steps` - Where to append the generated steps.

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

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

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
