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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxToolchainDescriptionArg {#class-cxxtoolchaindescriptionarg .title title="Class CxxToolchainDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxToolchainDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class CxxToolchainDescriptionArg
        extends Object

    ::: block
    This is roughly analagous to the configuration provided by
    `CxxBuckConfig`. Some things are not yet exposed/implemented, and
    others have been slightly renamed or exposed slightly differently to
    be more restricted or more descriptive or more maintainable.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CxxToolchainDe       | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`CxxToolchai         |
        |                       |                       | nDescriptionArg`](Cxx |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `builder()`           | ::: block             |
        | static CxxToolchainDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`CxxToolchai         |
        |                       |                       | nDescriptionArg`](Cxx |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `CxxToo               |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getArchiver()`       | ::: block             |
        |                       |                       | Archiver binary.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getArchiverFlags()`  | ::: block             |
        | ogle.common.collect.I |                       | Archiver flags.       |
        | mmutableList<String>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `getArchiverType()`   | ::: block             |
        | rchiverProvider.Type` |                       | [`ArchiverProvider.Ty |
        |                       |                       | pe`](toolchain/Archiv |
        |                       |                       | erProvider.Type.html  |
        |                       |                       | "enum in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |                       | of the archiver.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getAssembler()`      | ::: block             |
        |                       |                       | Assembler binary.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getAssemblerFlags()` | ::: block             |
        | ogle.common.collect.I |                       | Flags for the         |
        | mmutableList<String>` |                       | assembler.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     | ::: block             |
        |                       | getBinaryExtension()` | Extension for binary  |
        |                       |                       | files.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getCCompiler()`      | ::: block             |
        |                       |                       | C compiler binary.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCCompilerFlags()` | ::: block             |
        | ogle.common.collect.I |                       | C compiler flags.     |
        | mmutableList<String>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getCompilerType()`   | ::: block             |
        | CxxToolProvider.Type` |                       | [`CxxToolProvider.T   |
        |                       |                       | ype`](toolchain/CxxTo |
        |                       |                       | olProvider.Type.html  |
        |                       |                       | "enum in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |                       | of the compiler.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getCxxCompiler()`    | ::: block             |
        |                       |                       | C++ compiler binary.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    | ::: block             |
        | ogle.common.collect.I | etCxxCompilerFlags()` | C++ compiler flags.   |
        | mmutableList<String>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getFil               | ::: block             |
        |                       | epathLengthLimited()` | Whether to use        |
        |                       |                       | shorter intermediate  |
        |                       |                       | files.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    | ::: block             |
        | ogle.common.collect.I | etHeadersWhitelist()` | A list of regexes     |
        | mmutableList<String>` |                       | which match headers   |
        |                       |                       | (belonging to the     |
        |                       |                       | toolchain) to exempt  |
        |                       |                       | from untracked header |
        |                       |                       | verification.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getLinker()`         | ::: block             |
        |                       |                       | Linker binary.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getLinkerFlags()`    | ::: block             |
        | ogle.common.collect.I |                       | Linker flags.         |
        | mmutableList<String>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LinkerProvider.Type` | `getLinkerType()`     | ::: block             |
        |                       |                       | [`LinkerPr            |
        |                       |                       | ovider.Type`](toolcha |
        |                       |                       | in/linker/LinkerProvi |
        |                       |                       | der.Type.html "enum i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | xx.toolchain.linker") |
        |                       |                       | of the linker.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getNm()`             | ::: block             |
        |                       |                       | nm binary.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getObjcopyForShar    | ::: block             |
        |                       | edLibraryInterface()` | Objcopy binary to use |
        |                       |                       | for creating shared   |
        |                       |                       | library interfaces.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getO                 | ::: block             |
        |                       | bjectFileExtension()` | Extension for object  |
        |                       |                       | files.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getPrivateHead       | ::: block             |
        |                       | ersSymlinksEnabled()` | When building or      |
        |                       |                       | creating a project,   |
        |                       |                       | create symlinks for   |
        |                       |                       | the public headers if |
        |                       |                       | it\'s true.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getPublicHead        | ::: block             |
        |                       | ersSymlinksEnabled()` | When building or      |
        |                       |                       | creating a project,   |
        |                       |                       | create symlinks for   |
        |                       |                       | the public headers if |
        |                       |                       | it\'s true.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getRanlib()`         | ::: block             |
        | Optional<SourcePath>` |                       | Ranlib binary.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRanlibFlags()`    | ::: block             |
        | ogle.common.collect.I |                       | Ranlib flags.         |
        | mmutableList<String>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getShare             | ::: block             |
        | ogle.common.collect.I | dDepRuntimeLdFlags()` | Flags for linking the |
        | mmutableList<String>` |                       | c/c++ runtime for     |
        |                       |                       | shared libraries.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShar              | ::: block             |
        |                       | edLibraryExtension()` | Extension of shared   |
        |                       |                       | library files.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SharedLibrary        | `getSharedLi          | ::: block             |
        | InterfaceParams.Type` | braryInterfaceType()` | Type of shared        |
        |                       |                       | library interfaces to |
        |                       |                       | create.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    | ::: block             |
        |                       | etSharedLibraryVersio | Extension format for  |
        |                       | nedExtensionFormat()` | versioned shared      |
        |                       |                       | libraries.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getStati             | ::: block             |
        | ogle.common.collect.I | cDepRuntimeLdFlags()` | Flags for linking the |
        | mmutableList<String>` |                       | c/c++ runtime for     |
        |                       |                       | static libraries.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStat              | ::: block             |
        |                       | icLibraryExtension()` | Extension for static  |
        |                       |                       | library files.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getStaticPi          | ::: block             |
        | ogle.common.collect.I | cDepRuntimeLdFlags()` | Flags for linking the |
        | mmutableList<String>` |                       | c/c++ runtime for     |
        |                       |                       | static-pic libraries. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getStrip()`          | ::: block             |
        |                       |                       | Strip binary.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getStripFlags()`     | ::: block             |
        | ogle.common.collect.I |                       | Strip flags.          |
        | mmutableList<String>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUseArgFile()`     | ::: block             |
        |                       |                       | Whether to use an     |
        |                       |                       | argfile for long      |
        |                       |                       | command lines.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUseHeaderMap()`   | ::: block             |
        |                       |                       | Whether to use header |
        |                       |                       | maps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `privateHea           |
        |                       |                       | dersSymlinksEnabled`, |
        |                       |                       | `publicHea            |
        |                       |                       | dersSymlinksEnabled`, |
        |                       |                       | `useArgFile`,         |
        |                       |                       | `sha                  |
        |                       |                       | redLibraryExtension`, |
        |                       |                       | `sharedLibraryVersi   |
        |                       |                       | onedExtensionFormat`, |
        |                       |                       | `sta                  |
        |                       |                       | ticLibraryExtension`, |
        |                       |                       | `                     |
        |                       |                       | objectFileExtension`, |
        |                       |                       | `binaryExtension`,    |
        |                       |                       | `compilerType`,       |
        |                       |                       | `linkerType`,         |
        |                       |                       | `assembler`,          |
        |                       |                       | `assemblerFlags`,     |
        |                       |                       | `cCompiler`,          |
        |                       |                       | `cCompilerFlags`,     |
        |                       |                       | `cxxCompiler`,        |
        |                       |                       | `cxxCompilerFlags`,   |
        |                       |                       | `linker`,             |
        |                       |                       | `linkerFlags`,        |
        |                       |                       | `archiver`,           |
        |                       |                       | `archiverFlags`,      |
        |                       |                       | `archiverType`,       |
        |                       |                       | `strip`, `ranlib`,    |
        |                       |                       | `ranlibFlags`,        |
        |                       |                       | `stripFlags`,         |
        |                       |                       | `stat                 |
        |                       |                       | icDepRuntimeLdFlags`, |
        |                       |                       | `staticP              |
        |                       |                       | icDepRuntimeLdFlags`, |
        |                       |                       | `shar                 |
        |                       |                       | edDepRuntimeLdFlags`, |
        |                       |                       | `nm`,                 |
        |                       |                       | `sharedL              |
        |                       |                       | ibraryInterfaceType`, |
        |                       |                       | `objcopyForSha        |
        |                       |                       | redLibraryInterface`, |
        |                       |                       | `useHeaderMap`,       |
        |                       |                       | `fi                   |
        |                       |                       | lepathLengthLimited`, |
        |                       |                       | `headersWhitelist`,   |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `CxxToo               |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPrivateHeadersSymlinksEnabled()}

        -   #### getPrivateHeadersSymlinksEnabled

            ``` methodSignature
            public boolean getPrivateHeadersSymlinksEnabled()
            ```

            ::: block
            When building or creating a project, create symlinks for the
            public headers if it\'s true.
            :::

        []{#getPublicHeadersSymlinksEnabled()}

        -   #### getPublicHeadersSymlinksEnabled

            ``` methodSignature
            public boolean getPublicHeadersSymlinksEnabled()
            ```

            ::: block
            When building or creating a project, create symlinks for the
            public headers if it\'s true. It would allow public headers
            to include an other public header with #include
            \"foobar.h\"\\ even if it\'s not in the same folder.
            :::

        []{#getUseArgFile()}

        -   #### getUseArgFile

            ``` methodSignature
            public boolean getUseArgFile()
            ```

            ::: block
            Whether to use an argfile for long command lines.
            :::

        []{#getSharedLibraryExtension()}

        -   #### getSharedLibraryExtension

            ``` methodSignature
            public String getSharedLibraryExtension()
            ```

            ::: block
            Extension of shared library files.
            :::

        []{#getSharedLibraryVersionedExtensionFormat()}

        -   #### getSharedLibraryVersionedExtensionFormat

            ``` methodSignature
            public String getSharedLibraryVersionedExtensionFormat()
            ```

            ::: block
            Extension format for versioned shared libraries.
            :::

        []{#getStaticLibraryExtension()}

        -   #### getStaticLibraryExtension

            ``` methodSignature
            public String getStaticLibraryExtension()
            ```

            ::: block
            Extension for static library files.
            :::

        []{#getObjectFileExtension()}

        -   #### getObjectFileExtension

            ``` methodSignature
            public String getObjectFileExtension()
            ```

            ::: block
            Extension for object files.
            :::

        []{#getBinaryExtension()}

        -   #### getBinaryExtension

            ``` methodSignature
            public Optional<String> getBinaryExtension()
            ```

            ::: block
            Extension for binary files.
            :::

        []{#getCompilerType()}

        -   #### getCompilerType

            ``` methodSignature
            public CxxToolProvider.Type getCompilerType()
            ```

            ::: block
            [`CxxToolProvider.Type`](toolchain/CxxToolProvider.Type.html "enum in com.facebook.buck.cxx.toolchain")
            of the compiler.
            :::

        []{#getLinkerType()}

        -   #### getLinkerType

            ``` methodSignature
            public LinkerProvider.Type getLinkerType()
            ```

            ::: block
            [`LinkerProvider.Type`](toolchain/linker/LinkerProvider.Type.html "enum in com.facebook.buck.cxx.toolchain.linker")
            of the linker.
            :::

        []{#getAssembler()}

        -   #### getAssembler

            ``` methodSignature
            public SourcePath getAssembler()
            ```

            ::: block
            Assembler binary.
            :::

        []{#getAssemblerFlags()}

        -   #### getAssemblerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getAssemblerFlags()
            ```

            ::: block
            Flags for the assembler.
            :::

        []{#getCCompiler()}

        -   #### getCCompiler

            ``` methodSignature
            public SourcePath getCCompiler()
            ```

            ::: block
            C compiler binary.
            :::

        []{#getCCompilerFlags()}

        -   #### getCCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCCompilerFlags()
            ```

            ::: block
            C compiler flags.
            :::

        []{#getCxxCompiler()}

        -   #### getCxxCompiler

            ``` methodSignature
            public SourcePath getCxxCompiler()
            ```

            ::: block
            C++ compiler binary.
            :::

        []{#getCxxCompilerFlags()}

        -   #### getCxxCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCxxCompilerFlags()
            ```

            ::: block
            C++ compiler flags.
            :::

        []{#getLinker()}

        -   #### getLinker

            ``` methodSignature
            public SourcePath getLinker()
            ```

            ::: block
            Linker binary.
            :::

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getLinkerFlags()
            ```

            ::: block
            Linker flags.
            :::

        []{#getArchiver()}

        -   #### getArchiver

            ``` methodSignature
            public SourcePath getArchiver()
            ```

            ::: block
            Archiver binary.
            :::

        []{#getArchiverFlags()}

        -   #### getArchiverFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getArchiverFlags()
            ```

            ::: block
            Archiver flags.
            :::

        []{#getArchiverType()}

        -   #### getArchiverType

            ``` methodSignature
            public ArchiverProvider.Type getArchiverType()
            ```

            ::: block
            [`ArchiverProvider.Type`](toolchain/ArchiverProvider.Type.html "enum in com.facebook.buck.cxx.toolchain")
            of the archiver.
            :::

        []{#getStrip()}

        -   #### getStrip

            ``` methodSignature
            public SourcePath getStrip()
            ```

            ::: block
            Strip binary.
            :::

        []{#getRanlib()}

        -   #### getRanlib

            ``` methodSignature
            public Optional<SourcePath> getRanlib()
            ```

            ::: block
            Ranlib binary.
            :::

        []{#getRanlibFlags()}

        -   #### getRanlibFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getRanlibFlags()
            ```

            ::: block
            Ranlib flags.
            :::

        []{#getStripFlags()}

        -   #### getStripFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getStripFlags()
            ```

            ::: block
            Strip flags.
            :::

        []{#getStaticDepRuntimeLdFlags()}

        -   #### getStaticDepRuntimeLdFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getStaticDepRuntimeLdFlags()
            ```

            ::: block
            Flags for linking the c/c++ runtime for static libraries.
            :::

        []{#getStaticPicDepRuntimeLdFlags()}

        -   #### getStaticPicDepRuntimeLdFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getStaticPicDepRuntimeLdFlags()
            ```

            ::: block
            Flags for linking the c/c++ runtime for static-pic
            libraries.
            :::

        []{#getSharedDepRuntimeLdFlags()}

        -   #### getSharedDepRuntimeLdFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getSharedDepRuntimeLdFlags()
            ```

            ::: block
            Flags for linking the c/c++ runtime for shared libraries.
            :::

        []{#getNm()}

        -   #### getNm

            ``` methodSignature
            public SourcePath getNm()
            ```

            ::: block
            nm binary.
            :::

        []{#getSharedLibraryInterfaceType()}

        -   #### getSharedLibraryInterfaceType

            ``` methodSignature
            public SharedLibraryInterfaceParams.Type getSharedLibraryInterfaceType()
            ```

            ::: block
            Type of shared library interfaces to create.
            :::

        []{#getObjcopyForSharedLibraryInterface()}

        -   #### getObjcopyForSharedLibraryInterface

            ``` methodSignature
            public SourcePath getObjcopyForSharedLibraryInterface()
            ```

            ::: block
            Objcopy binary to use for creating shared library
            interfaces.
            :::

        []{#getUseHeaderMap()}

        -   #### getUseHeaderMap

            ``` methodSignature
            public boolean getUseHeaderMap()
            ```

            ::: block
            Whether to use header maps.
            :::

        []{#getFilepathLengthLimited()}

        -   #### getFilepathLengthLimited

            ``` methodSignature
            public boolean getFilepathLengthLimited()
            ```

            ::: block
            Whether to use shorter intermediate files.
            :::

        []{#getHeadersWhitelist()}

        -   #### getHeadersWhitelist

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getHeadersWhitelist()
            ```

            ::: block
            A list of regexes which match headers (belonging to the
            toolchain) to exempt from untracked header verification.
            :::

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `CxxToolchainDescriptionArg` that have equal attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes:
            `privateHeadersSymlinksEnabled`,
            `publicHeadersSymlinksEnabled`, `useArgFile`,
            `sharedLibraryExtension`,
            `sharedLibraryVersionedExtensionFormat`,
            `staticLibraryExtension`, `objectFileExtension`,
            `binaryExtension`, `compilerType`, `linkerType`,
            `assembler`, `assemblerFlags`, `cCompiler`,
            `cCompilerFlags`, `cxxCompiler`, `cxxCompilerFlags`,
            `linker`, `linkerFlags`, `archiver`, `archiverFlags`,
            `archiverType`, `strip`, `ranlib`, `ranlibFlags`,
            `stripFlags`, `staticDepRuntimeLdFlags`,
            `staticPicDepRuntimeLdFlags`, `sharedDepRuntimeLdFlags`,
            `nm`, `sharedLibraryInterfaceType`,
            `objcopyForSharedLibraryInterface`, `useHeaderMap`,
            `filepathLengthLimited`, `headersWhitelist`, `licenses`,
            `labels`, `defaultTargetPlatform`, `compatibleWith`, `name`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value `CxxToolchainDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CxxToolchainDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`CxxToolchainDescriptionArg`](CxxToolchainDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   A new CxxToolchainDescriptionArg builder
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
