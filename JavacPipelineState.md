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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavacPipelineState {#class-javacpipelinestate .title title="Class JavacPipelineState"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavacPipelineState

::: description
-   

    All Implemented Interfaces:
    :   `RulePipelineState`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class JavacPipelineState
        extends Object
        implements RulePipelineState
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavacPipelineState​(Javac javac,                   JavacOptions javacOptions,                   BuildTarget invokingRule,                   ClasspathChecker classpathChecker,                   CompilerParameters compilerParameters,                   JarParameters abiJarParameters,                   JarParameters libraryJarParameters)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Called after the      |
        |                       |                       | pipeline is done      |
        |                       |                       | (either through       |
        |                       |                       | success or failure    |
        |                       |                       | partway through) to   |
        |                       |                       | release resources.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Javac.Invocation`    | `                     | ::: block             |
        |                       | getJavacInvocation​(So | Get the invocation    |
        |                       | urcePathResolverAdapt | instance.             |
        |                       | er resolver,          | :::                   |
        |                       |           ProjectFile |                       |
        |                       | system filesystem,    |                       |
        |                       |                 Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `getO                 |                       |
        | ogle.common.collect.I | ptions​(JavacOptions j |                       |
        | mmutableList<String>` | avacOptions,          |                       |
        |                       |   ProjectFilesystem f |                       |
        |                       | ilesystem,            |                       |
        |                       | SourcePathResolverAda |                       |
        |                       | pter pathResolver,    |                       |
        |                       |         Path outputDi |                       |
        |                       | rectory,           Pa |                       |
        |                       | th generatedCodeDirec |                       |
        |                       | tory,           Execu |                       |
        |                       | tionContext context,  |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSortedSet<Path> bu |                       |
        |                       | ildClasspathEntries)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStderrContents()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStdoutContents()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRunning()`         |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.jvm.java.Javac,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.ClasspathChecker,com.facebook.buck.jvm.java.CompilerParameters,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters)}

        -   #### JavacPipelineState

                public JavacPipelineState​(Javac javac,
                                          JavacOptions javacOptions,
                                          BuildTarget invokingRule,
                                          ClasspathChecker classpathChecker,
                                          CompilerParameters compilerParameters,
                                          @Nullable
                                          JarParameters abiJarParameters,
                                          @Nullable
                                          JarParameters libraryJarParameters)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isRunning()}

        -   #### isRunning

            ``` methodSignature
            public boolean isRunning()
            ```

        []{#getJavacInvocation(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getJavacInvocation

            ``` methodSignature
            public Javac.Invocation getJavacInvocation​(SourcePathResolverAdapter resolver,
                                                       ProjectFilesystem filesystem,
                                                       ExecutionContext context)
                                                throws IOException
            ```

            ::: block
            Get the invocation instance.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getStdoutContents()}

        -   #### getStdoutContents

            ``` methodSignature
            public String getStdoutContents()
            ```

        []{#getStderrContents()}

        -   #### getStderrContents

            ``` methodSignature
            public String getStderrContents()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [Description copied from
            interface: `RulePipelineState`]{.descfrmTypeLabel}
            :::

            ::: block
            Called after the pipeline is done (either through success or
            failure partway through) to release resources.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `RulePipelineState`

        []{#getOptions(com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,java.nio.file.Path,com.facebook.buck.core.build.execution.context.ExecutionContext,com.google.common.collect.ImmutableSortedSet)}

        -   #### getOptions

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> getOptions​(JavacOptions javacOptions,
                                                                                     ProjectFilesystem filesystem,
                                                                                     SourcePathResolverAdapter pathResolver,
                                                                                     Path outputDirectory,
                                                                                     Path generatedCodeDirectory,
                                                                                     ExecutionContext context,
                                                                                     com.google.common.collect.ImmutableSortedSet<Path> buildClasspathEntries)
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
