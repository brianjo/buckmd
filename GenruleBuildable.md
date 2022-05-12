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

## Class GenruleBuildable {#class-genrulebuildable .title title="Class GenruleBuildable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.GenruleBuildable

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Buildable`

    ------------------------------------------------------------------------

        public class GenruleBuildable
        extends Object
        implements Buildable

    ::: block
    Buildable for
    [`Genrule`](Genrule.html "class in com.facebook.buck.shell")
    suitable for building Genrules directly and also for subclasses
    extending the functionality of a bare Genrule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `bash`                | ::: block             |
        | tected Optional<Arg>` |                       | The bash shell        |
        |                       |                       | command to generate   |
        |                       |                       | the output file.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `buildTarget`         | ::: block             |
        | rotected BuildTarget` |                       | The build target for  |
        |                       |                       | this genrule.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `cmd`                 | ::: block             |
        | tected Optional<Arg>` |                       | The shell command to  |
        |                       |                       | run to generate the   |
        |                       |                       | output file.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `cmdExe`              | ::: block             |
        | tected Optional<Arg>` |                       | The cmd shell command |
        |                       |                       | to generate the       |
        |                       |                       | output file.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `isCacheable`         | ::: block             |
        |                       |                       | Whether or not this   |
        |                       |                       | genrule can be        |
        |                       |                       | cached.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `out`                 | ::: block             |
        | ted Optional<String>` |                       | The name of the       |
        |                       |                       | output file that this |
        |                       |                       | genrule intends to    |
        |                       |                       | generate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Option     | `outputPath`          | ::: block             |
        | al<PublicOutputPath>` |                       | The output path of    |
        |                       |                       | the file generated by |
        |                       |                       | this genrule, if      |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Optional   | `outputPaths`         | ::: block             |
        | <com.google.common.co |                       | The output paths of   |
        | llect.ImmutableMap<Ou |                       | the files generated   |
        | tputLabel,​com.google. |                       | by this genrule       |
        | common.collect.Immuta |                       | organized by their    |
        | bleSet<OutputPath>>>` |                       | output labels.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Opti       | `outs`                | ::: block             |
        | onal<com.google.commo |                       | The names of the      |
        | n.collect.ImmutableMa |                       | output files that     |
        | p<OutputLabel,​com.goo |                       | this genrule intends  |
        | gle.common.collect.Im |                       | to generate relative  |
        | mutableSet<String>>>` |                       | to \$OUT mapped to    |
        |                       |                       | their respective      |
        |                       |                       | output group names.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `S                    | ::: block             |
        | tected static String` | RC_DIRECTORY_PATTERN` | Name of the \"srcs\"  |
        |                       |                       | subdirectory in the   |
        |                       |                       | gen directory tree.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected SourceSet` | `srcs`                | ::: block             |
        |                       |                       | SourceSet for this    |
        |                       |                       | Genrule, exposed as   |
        |                       |                       | SRCS in the genrule   |
        |                       |                       | command.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `type`                | ::: block             |
        | ted Optional<String>` |                       | Type for this         |
        |                       |                       | genrule, if one was   |
        |                       |                       | provided.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GenruleBuildable​(BuildTarget buildTarget,                 ProjectFilesystem filesystem,                 SandboxExecutionStrategy sandboxExecutionStrategy,                 SourceSet srcs,                 Optional<Arg> cmd,                 Optional<Arg> bash,                 Optional<Arg> cmdExe,                 Optional<String> type,                 Optional<String> out,                 Optional<com.google.common.collect.ImmutableMap<OutputLabel,​com.google.common.collect.ImmutableSet<String>>> outs,                 boolean enableSandboxingInGenrule,                 boolean isCacheable,                 String environmentExpansionSeparator,                 Optional<SandboxProperties> sandboxProperties,                 Optional<GenruleAndroidTools> androidTools,                 boolean executeRemotely)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addEnviron           | ::: block             |
        |                       | mentVariables​(SourceP | Adds the standard set |
        |                       | athResolverAdapter pa | of environment        |
        |                       | thResolver,           | variables to the      |
        |                       |               OutputP | genrule, which are    |
        |                       | athResolver outputPat | then exposed to the   |
        |                       | hResolver,            | genrule command.      |
        |                       |              ProjectF | :::                   |
        |                       | ilesystem filesystem, |                       |
        |                       |                       |                       |
        |                       |    Path srcPath,      |                       |
        |                       |                    Pa |                       |
        |                       | th tmpPath,           |                       |
        |                       |               com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableMap.Builder<St |                       |
        |                       | ring,​String> environm |                       |
        |                       | entVariablesBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getBuildSte          |                       |
        | google.common.collect | ps​(BuildContext build |                       |
        | .ImmutableList<Step>` | Context,              |                       |
        |                       |  ProjectFilesystem fi |                       |
        |                       | lesystem,             |                       |
        |                       |   OutputPathResolver  |                       |
        |                       | outputPathResolver,   |                       |
        |                       |             BuildCell |                       |
        |                       | RelativePathFactory b |                       |
        |                       | uildCellPathFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Arg>`       | `getCmd()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getOutputLabels()`   | ::: block             |
        | .common.collect.Immut |                       | Returns a set of      |
        | ableSet<OutputLabel>` |                       | output labels         |
        |                       |                       | associated with this  |
        |                       |                       | buildable.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getOutputName​(Outp   | ::: block             |
        |                       | utLabel outputLabel)` | Returns a String      |
        |                       |                       | representation of the |
        |                       |                       | output path relative  |
        |                       |                       | to the root output    |
        |                       |                       | directory.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getOutputs​(Outp      | ::: block             |
        | e.common.collect.Immu | utLabel outputLabel)` | Returns the set of    |
        | tableSet<OutputPath>` |                       | [`Out                 |
        |                       |                       | putPath`](../rules/mo |
        |                       |                       | dern/OutputPath.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.rules.modern") |
        |                       |                       | instances associated  |
        |                       |                       | with the given        |
        |                       |                       | [`Ou                  |
        |                       |                       | tputLabel`](../core/m |
        |                       |                       | odel/OutputLabel.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSet`           | `getSrcs()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `sho                  |                       |
        |                       | uldExecuteRemotely()` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#SRC_DIRECTORY_PATTERN}

        -   #### SRC_DIRECTORY_PATTERN

                protected static final String SRC_DIRECTORY_PATTERN

            ::: block
            Name of the \"srcs\" subdirectory in the gen directory tree.
            GenruleBuildable symlinks all source files into this
            directory and sets this directory to be the working
            directory of the command.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.shell.GenruleBuildable.SRC_DIRECTORY_PATTERN)

        []{#buildTarget}

        -   #### buildTarget

                protected final BuildTarget buildTarget

            ::: block
            The build target for this genrule.
            :::

        []{#srcs}

        -   #### srcs

                protected final SourceSet srcs

            ::: block
            SourceSet for this Genrule, exposed as SRCS in the genrule
            command.
            The order in which elements are specified in the `srcs`
            attribute of a genrule matters.
            :::

        []{#cmd}

        -   #### cmd

                protected final Optional<Arg> cmd

            ::: block
            The shell command to run to generate the output file. Used
            as the fallback if neither bash nor cmdExe are provided.
            :::

        []{#bash}

        -   #### bash

                protected final Optional<Arg> bash

            ::: block
            The bash shell command to generate the output file. Only
            used on platforms that have bash.
            :::

        []{#cmdExe}

        -   #### cmdExe

                protected final Optional<Arg> cmdExe

            ::: block
            The cmd shell command to generate the output file. Only used
            on Windows.
            :::

        []{#out}

        -   #### out

                protected final Optional<String> out

            ::: block
            The name of the output file that this genrule intends to
            generate. One and only one of [`out`](#out) and
            [`outs`](#outs) must be present.
            :::

        []{#outs}

        -   #### outs

                protected final Optional<com.google.common.collect.ImmutableMap<OutputLabel,​com.google.common.collect.ImmutableSet<String>>> outs

            ::: block
            The names of the output files that this genrule intends to
            generate relative to \$OUT mapped to their respective output
            group names.
            :::

        []{#outputPath}

        -   #### outputPath

                protected final Optional<PublicOutputPath> outputPath

            ::: block
            The output path of the file generated by this genrule, if
            present. Note that this output path is Public because it
            uses a folder name that is exactly equal to the target name,
            unlike other MBRs which use the target name suffixed by the
            flavor (or \_\_ if no flavor is provided). This is for
            backwards compatability with users of Buck that have
            hardcoded their paths. One and only one of
            [`outputPath`](#outputPath) and
            [`outputPaths`](#outputPaths) must be present.
            :::

        []{#outputPaths}

        -   #### outputPaths

                protected final Optional<com.google.common.collect.ImmutableMap<OutputLabel,​com.google.common.collect.ImmutableSet<OutputPath>>> outputPaths

            ::: block
            The output paths of the files generated by this genrule
            organized by their output labels.
            The paths are relative to the directory buck-out/gen/\_\_.
            For example, if the target is named \"foo\", the output
            paths in this map would be relative to buck-out/gen/foo\_\_.
            Note that [`outputPath`](#outputPath) places the output in
            buck-out/gen/foo.

            One and only one of [`outputPath`](#outputPath) and
            [`outputPaths`](#outputPaths) must be present.
            :::

        []{#isCacheable}

        -   #### isCacheable

                protected final boolean isCacheable

            ::: block
            Whether or not this genrule can be cached. This is not used
            within this class, but is required to be a part of the rule
            key.
            :::

        []{#type}

        -   #### type

                protected final Optional<String> type

            ::: block
            Type for this genrule, if one was provided.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.sandbox.SandboxExecutionStrategy,com.facebook.buck.rules.coercer.SourceSet,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,boolean,boolean,java.lang.String,java.util.Optional,java.util.Optional,boolean)}

        -   #### GenruleBuildable

                public GenruleBuildable​(BuildTarget buildTarget,
                                        ProjectFilesystem filesystem,
                                        SandboxExecutionStrategy sandboxExecutionStrategy,
                                        SourceSet srcs,
                                        Optional<Arg> cmd,
                                        Optional<Arg> bash,
                                        Optional<Arg> cmdExe,
                                        Optional<String> type,
                                        Optional<String> out,
                                        Optional<com.google.common.collect.ImmutableMap<OutputLabel,​com.google.common.collect.ImmutableSet<String>>> outs,
                                        boolean enableSandboxingInGenrule,
                                        boolean isCacheable,
                                        String environmentExpansionSeparator,
                                        Optional<SandboxProperties> sandboxProperties,
                                        Optional<GenruleAndroidTools> androidTools,
                                        boolean executeRemotely)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputs(com.facebook.buck.core.model.OutputLabel)}

        -   #### getOutputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<OutputPath> getOutputs​(OutputLabel outputLabel)
            ```

            ::: block
            Returns the set of
            [`OutputPath`](../rules/modern/OutputPath.html "class in com.facebook.buck.rules.modern")
            instances associated with the given
            [`OutputLabel`](../core/model/OutputLabel.html "class in com.facebook.buck.core.model").
            If multiple outputs are available, returns either the
            default or named output group. The default output group is
            the set of all named outputs.

            If multiple outputs are not available, returns a set
            containing the single output.
            :::

        []{#getOutputLabels()}

        -   #### getOutputLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<OutputLabel> getOutputLabels()
            ```

            ::: block
            Returns a set of output labels associated with this
            buildable.
            :::

        []{#getOutputName(com.facebook.buck.core.model.OutputLabel)}

        -   #### getOutputName

            ``` methodSignature
            public String getOutputName​(OutputLabel outputLabel)
            ```

            ::: block
            Returns a String representation of the output path relative
            to the root output directory.
            :::

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                               ProjectFilesystem filesystem,
                                                                               OutputPathResolver outputPathResolver,
                                                                               BuildCellRelativePathFactory buildCellPathFactory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `Buildable`

        []{#getCmd()}

        -   #### getCmd

            ``` methodSignature
            public Optional<Arg> getCmd()
            ```

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public SourceSet getSrcs()
            ```

        []{#shouldExecuteRemotely()}

        -   #### shouldExecuteRemotely

            ``` methodSignature
            public final boolean shouldExecuteRemotely()
            ```

        []{#addEnvironmentVariables(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableMap.Builder)}

        -   #### addEnvironmentVariables

            ``` methodSignature
            public void addEnvironmentVariables​(SourcePathResolverAdapter pathResolver,
                                                OutputPathResolver outputPathResolver,
                                                ProjectFilesystem filesystem,
                                                Path srcPath,
                                                Path tmpPath,
                                                com.google.common.collect.ImmutableMap.Builder<String,​String> environmentVariablesBuilder)
            ```

            ::: block
            Adds the standard set of environment variables to the
            genrule, which are then exposed to the genrule command.
            This method populates these well-known environment
            variables:

            -   `SRCS`, a delimited list of source file inputs to the
                genrule
            -   `OUT`, the genrule\'s output file
            -   `GEN_DIR`, Buck\'s gendir
            -   `SRCDIR`, the symlink-populated source directory
                readable to the command
            -   `TMP`, the temp directory usable by the command
            -   `ANDROID_HOME`, deprecated, the path to the Android SDK
                (if present)
            -   `ANDROID_SDK_ROOT`, the path to the Android SDK (if
                present)
            -   `DX`, the path to the Android DX executable (if present)
            -   `ZIPALIGN`, the path to the Android Zipalign executable
                (if present)
            -   `AAPT`, the path to the Android AAPT executable (if
                present)
            -   `AAPT2`, the path to the Android AAPT2 executable (if
                present)
            -   `NDK_HOME`, the path to the Android NDK (if present)

            This method also sets `NO_BUCKD` to `1`.
            :::

            [Parameters:]{.paramLabel}
            :   `pathResolver` - Path resolver for resolving paths for
                `SRCS`
            :   `outputPathResolver` - Path resolver for resolving `OUT`
            :   `filesystem` - Filesystem for resolving relative paths
                for `SRCDIR` and `TMP      `
            :   `srcPath` - Path to the generated symlink source
                directory
            :   `tmpPath` - Path to the genrule temporary directory
            :   `environmentVariablesBuilder` - Environment map builder
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
