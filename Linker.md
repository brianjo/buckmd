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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.linker](package-summary.html)
:::

## Interface Linker {#interface-linker .title title="Interface Linker"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Tool`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DarwinLinker`, `GnuLinker`, `WindowsLinker`

    ------------------------------------------------------------------------

        public interface Linker
        extends Tool

    ::: block
    An object wrapping a linker, providing its source path and an
    interface to decorate arguments with specific flags.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `L                    | ::: block             |
        |                       | inker.CxxRuntimeType` | The various styles of |
        |                       |                       | runtime library to    |
        |                       |                       | which we can link     |
        |                       |                       | shared objects.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Linker               | ::: block             |
        |                       | .ExtraOutputsDeriver` | Derives extra outputs |
        |                       |                       | from linker args      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Li                   | ::: block             |
        |                       | nker.LinkableDepType` | The various ways to   |
        |                       |                       | link in dependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Linker.LinkType`     | ::: block             |
        |                       |                       | The various ways to   |
        |                       |                       | link an output file.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Linker.Shar          | ::: block             |
        |                       | edLibraryLoadingType` | The various ways to   |
        |                       |                       | load shared libraries |
        |                       |                       | on different          |
        |                       |                       | platforms             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com                  | `createUndefinedSym   | ::: block             |
        | .google.common.collec | bolsLinkerArgs​(Projec | Generate a necessary  |
        | t.ImmutableList<Arg>` | tFilesystem projectFi | linker arguments to   |
        |                       | lesystem,             | propagate undefined   |
        |                       |                       | symbols to a link     |
        |                       | BuildRuleParams baseP | command.              |
        |                       | arams,                | :::                   |
        |                       |                   Act |                       |
        |                       | ionGraphBuilder graph |                       |
        |                       | Builder,              |                       |
        |                       |                     B |                       |
        |                       | uildTarget target,    |                       |
        |                       |                       |                       |
        |                       |          com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leList<? extends Sour |                       |
        |                       | cePath> symbolFiles)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `d                    | `fileList​(A           | ::: block             |
        | efault Iterable<Arg>` | bsPath fileListPath)` | Abs-path version of   |
        |                       |                       | [`fileLi              |
        |                       |                       | st(Path)`](#fileList( |
        |                       |                       | java.nio.file.Path)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `fileLis              | ::: block             |
        |                       | t​(Path fileListPath)` | Specifies that the    |
        |                       |                       | linker should link    |
        |                       |                       | the files listed in   |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Linker.     | `getE                 |                       |
        | ExtraOutputsDeriver>` | xtraOutputsDeriver()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<String>`    | `getIgnoreUnd         |                       |
        |                       | efinedSymbolsFlags()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<String>`    | `getNoAsNee           |                       |
        |                       | dedSharedLibsFlags()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getScrubbers​(        |                       |
        | ommon.collect.Immutab | com.google.common.col |                       |
        | leList<FileScrubber>` | lect.ImmutableMap<Pat |                       |
        |                       | h,​Path> cellRootMap)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `getSharedLibFlag()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Linker.Shar          | `getShared            |                       |
        | edLibraryLoadingType` | LibraryLoadingType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUs                |                       |
        |                       | eUnixPathSeparator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `libOrigin()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `lin                  |                       |
        |                       | kWhole​(Arg input,     |                       |
        |                       |       SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `origin()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<String>`    | `out                  |                       |
        |                       | putArgs​(String path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `preloadEnvVar()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `searchPathEnvVar()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<String>`    | `s                    |                       |
        |                       | oname​(String soname)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScrubbers(com.google.common.collect.ImmutableMap)}

        -   #### getScrubbers

            ``` methodSignature
            com.google.common.collect.ImmutableList<FileScrubber> getScrubbers​(com.google.common.collect.ImmutableMap<Path,​Path> cellRootMap)
            ```

            [Parameters:]{.paramLabel}
            :   `cellRootMap` - Replacement map for cell roots found in
                paths, to some suitably normalized form (such as a
                relative path from root cell).

        []{#linkWhole(com.facebook.buck.rules.args.Arg,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### linkWhole

            ``` methodSignature
            Iterable<Arg> linkWhole​(Arg input,
                                    SourcePathResolverAdapter resolver)
            ```

            [Returns:]{.returnLabel}
            :   the platform-specific way to specify that the library
                represented by the given argument should be linked
                whole.

        []{#soname(java.lang.String)}

        -   #### soname

            ``` methodSignature
            Iterable<String> soname​(String soname)
            ```

            [Returns:]{.returnLabel}
            :   the platform-specific way to specify that linker should
                use the given soname when linking a shared library.

        []{#fileList(java.nio.file.Path)}

        -   #### fileList

            ``` methodSignature
            Iterable<Arg> fileList​(Path fileListPath)
            ```

            ::: block
            Specifies that the linker should link the files listed in
            file. This is an alternative to listing the files on the
            command line. The file names are listed one per line
            separated only by newlines. Spaces and tabs are assumed to
            be part of the file name.
            :::

            [Parameters:]{.paramLabel}
            :   `fileListPath` - the path to file which contains
                contents for file list to link

            [Returns:]{.returnLabel}
            :   the platform-specific way to support the feature. Empty
                list if feature is not supported.

        []{#fileList(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### fileList

            ``` methodSignature
            default Iterable<Arg> fileList​(AbsPath fileListPath)
            ```

            ::: block
            Abs-path version of
            [`fileList(Path)`](#fileList(java.nio.file.Path)).
            :::

        []{#origin()}

        -   #### origin

            ``` methodSignature
            String origin()
            ```

            [Returns:]{.returnLabel}
            :   the placeholder used by the dynamic loader for the
                directory containing the top-level executable.

        []{#libOrigin()}

        -   #### libOrigin

            ``` methodSignature
            String libOrigin()
            ```

            [Returns:]{.returnLabel}
            :   the placeholder used by the dynamic loader for the
                directory containing the top-level library (useful for
                e.g. plugins).

        []{#searchPathEnvVar()}

        -   #### searchPathEnvVar

            ``` methodSignature
            String searchPathEnvVar()
            ```

            [Returns:]{.returnLabel}
            :   the name of the environment variable for the shared
                library runtime search path.

        []{#preloadEnvVar()}

        -   #### preloadEnvVar

            ``` methodSignature
            String preloadEnvVar()
            ```

            [Returns:]{.returnLabel}
            :   the name of the environment variable for the shared
                library preload search path.

        []{#getNoAsNeededSharedLibsFlags()}

        -   #### getNoAsNeededSharedLibsFlags

            ``` methodSignature
            Iterable<String> getNoAsNeededSharedLibsFlags()
            ```

            [Returns:]{.returnLabel}
            :   arguments to pass to the linker to disable dropping
                runtime references to shared libs which do not resolve
                symbols as link-time.

        []{#getIgnoreUndefinedSymbolsFlags()}

        -   #### getIgnoreUndefinedSymbolsFlags

            ``` methodSignature
            Iterable<String> getIgnoreUndefinedSymbolsFlags()
            ```

            [Returns:]{.returnLabel}
            :   arguments to pass to the linker so that it ignores
                undefined symbols when linking.

        []{#createUndefinedSymbolsLinkerArgs(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList)}

        -   #### createUndefinedSymbolsLinkerArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> createUndefinedSymbolsLinkerArgs​(ProjectFilesystem projectFilesystem,
                                                                                          BuildRuleParams baseParams,
                                                                                          ActionGraphBuilder graphBuilder,
                                                                                          BuildTarget target,
                                                                                          com.google.common.collect.ImmutableList<? extends SourcePath> symbolFiles)
            ```

            ::: block
            Generate a necessary linker arguments to propagate undefined
            symbols to a link command. May need to create a
            [`BuildRule`](../../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"),
            in which case, `target` will be used as its name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - the name to give any
                [`BuildRule`](../../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that needs to be created to facilitate generating the
                arguments,
            :   `symbolFiles` - the symbols files, each listing
                undefined symbols, one per line, to add to the link.

            [Returns:]{.returnLabel}
            :   the list of linker arguments needed to propagate the
                list of undefined symbols to the link command.

        []{#getSharedLibFlag()}

        -   #### getSharedLibFlag

            ``` methodSignature
            Iterable<Arg> getSharedLibFlag()
            ```

        []{#outputArgs(java.lang.String)}

        -   #### outputArgs

            ``` methodSignature
            Iterable<String> outputArgs​(String path)
            ```

        []{#getSharedLibraryLoadingType()}

        -   #### getSharedLibraryLoadingType

            ``` methodSignature
            Linker.SharedLibraryLoadingType getSharedLibraryLoadingType()
            ```

        []{#getExtraOutputsDeriver()}

        -   #### getExtraOutputsDeriver

            ``` methodSignature
            Optional<Linker.ExtraOutputsDeriver> getExtraOutputsDeriver()
            ```

        []{#getUseUnixPathSeparator()}

        -   #### getUseUnixPathSeparator

            ``` methodSignature
            boolean getUseUnixPathSeparator()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
