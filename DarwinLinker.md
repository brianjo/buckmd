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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.linker.impl](package-summary.html)
:::

## Class DarwinLinker {#class-darwinlinker .title title="Class DarwinLinker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.tool.DelegatingTool](../../../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

    -   -   com.facebook.buck.cxx.toolchain.linker.impl.DarwinLinker

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `HasIncrementalThinLTO`,
        `HasLinkerMap`, `HasLTO`, `Linker`

    ------------------------------------------------------------------------

        public class DarwinLinker
        extends DelegatingTool
        implements Linker, HasLinkerMap, HasIncrementalThinLTO, HasLTO

    ::: block
    A specialization of
    [`Linker`](../Linker.html "interface in com.facebook.buck.cxx.toolchain.linker")
    containing information specific to the Darwin implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.linker.Linker}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.linker.[Linker](../Linker.html "interface in com.facebook.buck.cxx.toolchain.linker")

            `Linker.CxxRuntimeType, Linker.ExtraOutputsDeriver, Linker.LinkableDepType, Linker.LinkType, Linker.SharedLibraryLoadingType`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                        Description
          -------------------------------------------------------------------------------------------------- -------------
          `DarwinLinker​(Tool tool,             boolean cacheLinks,             boolean scrubConcurrently)`    

          : Constructors[ ]{.tabEnd}
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
        | `Iterable<Arg>`       | `fatLTO​(Path output)` |                       |
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
        | `Iterable<Arg>`       | `incrementalThinL     |                       |
        |                       | TOFlags​(Path output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `libOrigin()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `li                   |                       |
        |                       | nkerMap​(Path output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `linker               |                       |
        |                       | MapPath​(Path output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `lin                  |                       |
        |                       | kWhole​(Arg input,     |                       |
        |                       |       SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `                     |                       |
        |                       | ltoPath​(Path output)` |                       |
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
        | `Iterable<String>`    | `soname​(String arg)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `                     |                       |
        |                       | thinLTO​(Path output)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.DelegatingTool}

            ### Methods inherited from class com.facebook.buck.core.toolchain.tool.[DelegatingTool](../../../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.linker.Linker}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.linker.[Linker](../Linker.html "interface in com.facebook.buck.cxx.toolchain.linker")

            `fileList`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool,boolean,boolean)}

        -   #### DarwinLinker

                public DarwinLinker​(Tool tool,
                                    boolean cacheLinks,
                                    boolean scrubConcurrently)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScrubbers(com.google.common.collect.ImmutableMap)}

        -   #### getScrubbers

            ``` methodSignature
            public com.google.common.collect.ImmutableList<FileScrubber> getScrubbers​(com.google.common.collect.ImmutableMap<Path,​Path> cellRootMap)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getScrubbers` in interface `Linker`

            [Parameters:]{.paramLabel}
            :   `cellRootMap` - Replacement map for cell roots found in
                paths, to some suitably normalized form (such as a
                relative path from root cell).

        []{#linkWhole(com.facebook.buck.rules.args.Arg,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### linkWhole

            ``` methodSignature
            public Iterable<Arg> linkWhole​(Arg input,
                                           SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `linkWhole` in interface `Linker`

            [Returns:]{.returnLabel}
            :   the platform-specific way to specify that the library
                represented by the given argument should be linked
                whole.

        []{#linkerMap(java.nio.file.Path)}

        -   #### linkerMap

            ``` methodSignature
            public Iterable<Arg> linkerMap​(Path output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `linkerMap` in interface `HasLinkerMap`

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the platform-specific way to generate a link-map file.

        []{#linkerMapPath(java.nio.file.Path)}

        -   #### linkerMapPath

            ``` methodSignature
            public Path linkerMapPath​(Path output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `linkerMapPath` in interface `HasLinkerMap`

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the path of the output binary\'s link-map file generated
                by the linker.

        []{#thinLTO(java.nio.file.Path)}

        -   #### thinLTO

            ``` methodSignature
            public Iterable<Arg> thinLTO​(Path output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `thinLTO` in interface `HasLTO`

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the platform-specific way to set the path for thin lto
                object files.

        []{#incrementalThinLTOFlags(java.nio.file.Path)}

        -   #### incrementalThinLTOFlags

            ``` methodSignature
            public Iterable<Arg> incrementalThinLTOFlags​(Path output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `incrementalThinLTOFlags` in
                interface `HasIncrementalThinLTO`

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output index files

            [Returns:]{.returnLabel}
            :   the platform-specific way to generate intermediate build
                products for ThinLTO.

        []{#fatLTO(java.nio.file.Path)}

        -   #### fatLTO

            ``` methodSignature
            public Iterable<Arg> fatLTO​(Path output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fatLTO` in interface `HasLTO`

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the platform-specific way to set the path for monolithic
                lto object files.

        []{#ltoPath(java.nio.file.Path)}

        -   #### ltoPath

            ``` methodSignature
            public Path ltoPath​(Path output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `ltoPath` in interface `HasLTO`

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the path of the lto object files generated by the
                linker.

        []{#soname(java.lang.String)}

        -   #### soname

            ``` methodSignature
            public Iterable<String> soname​(String arg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `soname` in interface `Linker`

            [Returns:]{.returnLabel}
            :   the platform-specific way to specify that linker should
                use the given soname when linking a shared library.

        []{#fileList(java.nio.file.Path)}

        -   #### fileList

            ``` methodSignature
            public Iterable<Arg> fileList​(Path fileListPath)
            ```

            ::: block
            [Description copied from
            interface: `Linker`]{.descfrmTypeLabel}
            :::

            ::: block
            Specifies that the linker should link the files listed in
            file. This is an alternative to listing the files on the
            command line. The file names are listed one per line
            separated only by newlines. Spaces and tabs are assumed to
            be part of the file name.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `fileList` in interface `Linker`

            [Parameters:]{.paramLabel}
            :   `fileListPath` - the path to file which contains
                contents for file list to link

            [Returns:]{.returnLabel}
            :   the platform-specific way to support the feature. Empty
                list if feature is not supported.

        []{#origin()}

        -   #### origin

            ``` methodSignature
            public String origin()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `origin` in interface `Linker`

            [Returns:]{.returnLabel}
            :   the placeholder used by the dynamic loader for the
                directory containing the top-level executable.

        []{#libOrigin()}

        -   #### libOrigin

            ``` methodSignature
            public String libOrigin()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `libOrigin` in interface `Linker`

            [Returns:]{.returnLabel}
            :   the placeholder used by the dynamic loader for the
                directory containing the top-level library (useful for
                e.g. plugins).

        []{#searchPathEnvVar()}

        -   #### searchPathEnvVar

            ``` methodSignature
            public String searchPathEnvVar()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `searchPathEnvVar` in interface `Linker`

            [Returns:]{.returnLabel}
            :   the name of the environment variable for the shared
                library runtime search path.

        []{#preloadEnvVar()}

        -   #### preloadEnvVar

            ``` methodSignature
            public String preloadEnvVar()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `preloadEnvVar` in interface `Linker`

            [Returns:]{.returnLabel}
            :   the name of the environment variable for the shared
                library preload search path.

        []{#createUndefinedSymbolsLinkerArgs(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList)}

        -   #### createUndefinedSymbolsLinkerArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Arg> createUndefinedSymbolsLinkerArgs​(ProjectFilesystem projectFilesystem,
                                                                                                 BuildRuleParams baseParams,
                                                                                                 ActionGraphBuilder graphBuilder,
                                                                                                 BuildTarget target,
                                                                                                 com.google.common.collect.ImmutableList<? extends SourcePath> symbolFiles)
            ```

            ::: block
            [Description copied from
            interface: `Linker`]{.descfrmTypeLabel}
            :::

            ::: block
            Generate a necessary linker arguments to propagate undefined
            symbols to a link command. May need to create a
            [`BuildRule`](../../../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"),
            in which case, `target` will be used as its name.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createUndefinedSymbolsLinkerArgs` in interface `Linker`
            :   `target` - the name to give any
                [`BuildRule`](../../../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that needs to be created to facilitate generating the
                arguments,
            :   `symbolFiles` - the symbols files, each listing
                undefined symbols, one per line, to add to the link.

            [Returns:]{.returnLabel}
            :   the list of linker arguments needed to propagate the
                list of undefined symbols to the link command.

        []{#getNoAsNeededSharedLibsFlags()}

        -   #### getNoAsNeededSharedLibsFlags

            ``` methodSignature
            public Iterable<String> getNoAsNeededSharedLibsFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNoAsNeededSharedLibsFlags` in interface `Linker`

            [Returns:]{.returnLabel}
            :   arguments to pass to the linker to disable dropping
                runtime references to shared libs which do not resolve
                symbols as link-time.

        []{#getIgnoreUndefinedSymbolsFlags()}

        -   #### getIgnoreUndefinedSymbolsFlags

            ``` methodSignature
            public Iterable<String> getIgnoreUndefinedSymbolsFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIgnoreUndefinedSymbolsFlags` in interface `Linker`

            [Returns:]{.returnLabel}
            :   arguments to pass to the linker so that it ignores
                undefined symbols when linking.

        []{#getSharedLibFlag()}

        -   #### getSharedLibFlag

            ``` methodSignature
            public Iterable<Arg> getSharedLibFlag()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSharedLibFlag` in interface `Linker`

        []{#outputArgs(java.lang.String)}

        -   #### outputArgs

            ``` methodSignature
            public Iterable<String> outputArgs​(String path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `outputArgs` in interface `Linker`

        []{#getSharedLibraryLoadingType()}

        -   #### getSharedLibraryLoadingType

            ``` methodSignature
            public Linker.SharedLibraryLoadingType getSharedLibraryLoadingType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSharedLibraryLoadingType` in interface `Linker`

        []{#getExtraOutputsDeriver()}

        -   #### getExtraOutputsDeriver

            ``` methodSignature
            public Optional<Linker.ExtraOutputsDeriver> getExtraOutputsDeriver()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraOutputsDeriver` in interface `Linker`

        []{#getUseUnixPathSeparator()}

        -   #### getUseUnixPathSeparator

            ``` methodSignature
            public boolean getUseUnixPathSeparator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUseUnixPathSeparator` in interface `Linker`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
