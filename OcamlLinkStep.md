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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlLinkStep {#class-ocamllinkstep .title title="Class OcamlLinkStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.features.ocaml.OcamlLinkStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class OcamlLinkStep
        extends ShellStep

    ::: block
    OCaml linking step. Dependencies and inputs should be topologically
    ordered
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                         Field                          Description
          --------------------------------------------------------- ------------------------------ -------------
          `Path`                                                    `argFile`                       
          `com.google.common.collect.ImmutableList<String>`         `cDepInput`                     
          `com.google.common.collect.ImmutableList<String>`         `cxxCompiler`                   
          `com.google.common.collect.ImmutableMap<String,​String>`   `environment`                   
          `ProjectFilesystem`                                       `filesystem`                    
          `com.google.common.collect.ImmutableList<String>`         `flags`                         
          `com.google.common.collect.ImmutableList<Path>`           `input`                         
          `boolean`                                                 `isBytecode`                    
          `boolean`                                                 `isLibrary`                     
          `com.google.common.collect.ImmutableList<String>`         `ocamlCompilerCommandPrefix`    
          `Path`                                                    `output`                        
          `Optional<String>`                                        `stdlib`                        

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Fields inherited from class com.facebook.buck.shell.[ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

            `workingDirectory`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `create​(ProjectF      | ::: block             |
        | static OcamlLinkStep` | ilesystem filesystem, | Factory method for    |
        |                       |        com.google.com | OcamlLinkStep.        |
        |                       | mon.collect.Immutable | :::                   |
        |                       | Map<String,​String> en |                       |
        |                       | vironment,       com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableList<String |                       |
        |                       | > cxxCompiler,        |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList<St |                       |
        |                       | ring> ocamlCompilerCo |                       |
        |                       | mmandPrefix,       co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableList<Arg> |                       |
        |                       |  flags,       Optiona |                       |
        |                       | l<String> stdlib,     |                       |
        |                       |    Path output,       |                       |
        |                       |  Path argFile,        |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList<Ar |                       |
        |                       | g> depInput,       co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableList<Arg> |                       |
        |                       |  cDepInput,       com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Path> |                       |
        |                       |  input,       boolean |                       |
        |                       |  isLibrary,       boo |                       |
        |                       | lean isBytecode,      |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](../../shell/ShellStep.html "class in com.facebook.buck.shell")

            `addOptions, execute, getDescription, getDuration, getExitCodeFromResult, getShellCommand, getShellCommandArgsForDescription, getStderr, getStdin, getStdout, getTimeout, getTimeoutHandler, shouldPrintStderr, shouldPrintStdout`

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

        []{#filesystem}

        -   #### filesystem

                public final ProjectFilesystem filesystem

        []{#environment}

        -   #### environment

                public final com.google.common.collect.ImmutableMap<String,​String> environment

        []{#cxxCompiler}

        -   #### cxxCompiler

                public final com.google.common.collect.ImmutableList<String> cxxCompiler

        []{#ocamlCompilerCommandPrefix}

        -   #### ocamlCompilerCommandPrefix

                public final com.google.common.collect.ImmutableList<String> ocamlCompilerCommandPrefix

        []{#flags}

        -   #### flags

                public final com.google.common.collect.ImmutableList<String> flags

        []{#stdlib}

        -   #### stdlib

                public final Optional<String> stdlib

        []{#output}

        -   #### output

                public final Path output

        []{#argFile}

        -   #### argFile

                public final Path argFile

        []{#cDepInput}

        -   #### cDepInput

                public final com.google.common.collect.ImmutableList<String> cDepInput

        []{#input}

        -   #### input

                public final com.google.common.collect.ImmutableList<Path> input

        []{#isLibrary}

        -   #### isLibrary

                public final boolean isLibrary

        []{#isBytecode}

        -   #### isBytecode

                public final boolean isBytecode
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,java.util.Optional,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,boolean,boolean,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### create

            ``` methodSignature
            public static OcamlLinkStep create​(ProjectFilesystem filesystem,
                                               com.google.common.collect.ImmutableMap<String,​String> environment,
                                               com.google.common.collect.ImmutableList<String> cxxCompiler,
                                               com.google.common.collect.ImmutableList<String> ocamlCompilerCommandPrefix,
                                               com.google.common.collect.ImmutableList<Arg> flags,
                                               Optional<String> stdlib,
                                               Path output,
                                               Path argFile,
                                               com.google.common.collect.ImmutableList<Arg> depInput,
                                               com.google.common.collect.ImmutableList<Arg> cDepInput,
                                               com.google.common.collect.ImmutableList<Path> input,
                                               boolean isLibrary,
                                               boolean isBytecode,
                                               SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            Factory method for OcamlLinkStep.
            :::

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
