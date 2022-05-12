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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface CxxPlatform {#interface-cxxplatform .title title="Interface CxxPlatform"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `FlavorConvertible`

    ------------------------------------------------------------------------

        public interface CxxPlatform
        extends FlavorConvertible

    ::: block
    Interface describing a C/C++ toolchain and platform to build for.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface               Description
          ------------------- ----------------------- -------------
          `static class `     `CxxPlatform.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `builder()`           |                       |
        |  CxxPlatform.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArchiverProvider`    | `getAr()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArchiveContents`     | `                     |                       |
        |                       | getArchiveContents()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getArflags()`        |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CompilerProvider`    | `getAs()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getAsflags()`        |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getAsm()`            |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getAsmflags()`       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getAsmpp()`          |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getAsmppflags()`     |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getAspp()`           |                       |
        | PreprocessorProvider` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getAsppflags()`      |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getBinaryExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CompilerProvider`    | `getCc()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getCflags()`         |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `DebugPathSanitizer`  | `getCompiler          |                       |
        |                       | DebugPathSanitizer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.google.  | `getConflictingHeade  |                       |
        | common.collect.Immuta | rBasenameWhitelist()` |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getCpp()`            |                       |
        | PreprocessorProvider` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getCppflags()`       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCuda()`           |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getCudaflags()`      |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getCudapp()`         |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getCudappflags()`    |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CompilerProvider`    | `getCxx()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getCxxflags()`       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getCxxpp()`          |                       |
        | PreprocessorProvider` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getCxxppflags()`     |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getFil               |                       |
        |                       | epathLengthLimited()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getFlagMacros()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getHeaderMode()`     |                       |
        | Optional<HeaderMode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HeaderVerification`  | `get                  |                       |
        |                       | HeaderVerification()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getHip()`            |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getHipflags()`       |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getHippp()`          |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getHipppflags()`     |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `LinkerProvider`      | `getLd()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getLdflags()`        |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getO                 |                       |
        |                       | bjectFileExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default PicType`     | `getPicTy             | ::: block             |
        |                       | peForSharedLinking()` | nix platforms use PIC |
        |                       |                       | object files for      |
        |                       |                       | shared libraries,     |
        |                       |                       | while windows         |
        |                       |                       | doesn\'t.             |
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
        | `Op                   | `getRanlib()`         |                       |
        | tional<ToolProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getRanlibflags()`    |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getRuntimeLdflags()` |                       |
        | e.common.collect.Immu |                       |                       |
        | tableMultimap<Linker. |                       |                       |
        | LinkableDepType,​Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShar              |                       |
        |                       | edLibraryExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<SharedLib   | `getSharedLibr        |                       |
        | raryInterfaceParams>` | aryInterfaceParams()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etSharedLibraryVersio |                       |
        |                       | nedExtensionFormat()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getStat              |                       |
        |                       | icLibraryExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getStrip()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getStripFlags()`     |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SymbolNameTool`      | `getSymbolNameTool()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getUseArgFile()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withArchive          |                       |
        |                       | Contents​(ArchiveConte |                       |
        |                       | nts archiveContents)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `wit                  |                       |
        |                       | hAsflags​(com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leList<Arg> asFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `w                    |                       |
        |                       | ithCflags​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleList<Arg> cFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withCompilerDeb      |                       |
        |                       | ugPathSanitizer​(Debug |                       |
        |                       | PathSanitizer compile |                       |
        |                       | rDebugPathSanitizer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `wi                   |                       |
        |                       | thConflictingHeaderBa |                       |
        |                       | senameWhitelist​(com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableSortedSet<St |                       |
        |                       | ring> conflictingHead |                       |
        |                       | erBasenameWhitelist)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withCpp​(Prepr        |                       |
        |                       | ocessorProvider cpp)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withC                |                       |
        |                       | ppflags​(com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<Arg> cppFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `w                    |                       |
        |                       | ithCxx​(CompilerProvid |                       |
        |                       | er compilerProvider)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withC                |                       |
        |                       | xxflags​(com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<Arg> cxxFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withCxxpp​(P          |                       |
        |                       | reprocessorProvider p |                       |
        |                       | reprocessorProvider)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withCxxpp            |                       |
        |                       | flags​(com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist<Arg> cxxppflags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withFlagMacros​(com   |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableMap<String |                       |
        |                       | ,​String> flagMacros)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default CxxPlatform` | `withF                |                       |
        |                       | lavor​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#getAs()}

        -   #### getAs

            ``` methodSignature
            CompilerProvider getAs()
            ```

        []{#getAsflags()}

        -   #### getAsflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getAsflags()
            ```

        []{#getAspp()}

        -   #### getAspp

            ``` methodSignature
            PreprocessorProvider getAspp()
            ```

        []{#getAsppflags()}

        -   #### getAsppflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getAsppflags()
            ```

        []{#getCc()}

        -   #### getCc

            ``` methodSignature
            CompilerProvider getCc()
            ```

        []{#getCflags()}

        -   #### getCflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getCflags()
            ```

        []{#getCxx()}

        -   #### getCxx

            ``` methodSignature
            CompilerProvider getCxx()
            ```

        []{#getCxxflags()}

        -   #### getCxxflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getCxxflags()
            ```

        []{#getCpp()}

        -   #### getCpp

            ``` methodSignature
            PreprocessorProvider getCpp()
            ```

        []{#getCppflags()}

        -   #### getCppflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getCppflags()
            ```

        []{#getCxxpp()}

        -   #### getCxxpp

            ``` methodSignature
            PreprocessorProvider getCxxpp()
            ```

        []{#getCxxppflags()}

        -   #### getCxxppflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getCxxppflags()
            ```

        []{#getCudapp()}

        -   #### getCudapp

            ``` methodSignature
            Optional<PreprocessorProvider> getCudapp()
            ```

        []{#getCudappflags()}

        -   #### getCudappflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getCudappflags()
            ```

        []{#getCuda()}

        -   #### getCuda

            ``` methodSignature
            Optional<CompilerProvider> getCuda()
            ```

        []{#getCudaflags()}

        -   #### getCudaflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getCudaflags()
            ```

        []{#getHippp()}

        -   #### getHippp

            ``` methodSignature
            Optional<PreprocessorProvider> getHippp()
            ```

        []{#getHipppflags()}

        -   #### getHipppflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getHipppflags()
            ```

        []{#getHip()}

        -   #### getHip

            ``` methodSignature
            Optional<CompilerProvider> getHip()
            ```

        []{#getHipflags()}

        -   #### getHipflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getHipflags()
            ```

        []{#getAsmpp()}

        -   #### getAsmpp

            ``` methodSignature
            Optional<PreprocessorProvider> getAsmpp()
            ```

        []{#getAsmppflags()}

        -   #### getAsmppflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getAsmppflags()
            ```

        []{#getAsm()}

        -   #### getAsm

            ``` methodSignature
            Optional<CompilerProvider> getAsm()
            ```

        []{#getAsmflags()}

        -   #### getAsmflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getAsmflags()
            ```

        []{#getLd()}

        -   #### getLd

            ``` methodSignature
            LinkerProvider getLd()
            ```

        []{#getLdflags()}

        -   #### getLdflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getLdflags()
            ```

        []{#getRuntimeLdflags()}

        -   #### getRuntimeLdflags

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<Linker.LinkableDepType,​Arg> getRuntimeLdflags()
            ```

        []{#getStrip()}

        -   #### getStrip

            ``` methodSignature
            Tool getStrip()
            ```

        []{#getStripFlags()}

        -   #### getStripFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getStripFlags()
            ```

        []{#getAr()}

        -   #### getAr

            ``` methodSignature
            ArchiverProvider getAr()
            ```

        []{#getArchiveContents()}

        -   #### getArchiveContents

            ``` methodSignature
            ArchiveContents getArchiveContents()
            ```

        []{#getArflags()}

        -   #### getArflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getArflags()
            ```

        []{#getRanlib()}

        -   #### getRanlib

            ``` methodSignature
            Optional<ToolProvider> getRanlib()
            ```

        []{#getRanlibflags()}

        -   #### getRanlibflags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getRanlibflags()
            ```

        []{#getSymbolNameTool()}

        -   #### getSymbolNameTool

            ``` methodSignature
            SymbolNameTool getSymbolNameTool()
            ```

        []{#getSharedLibraryExtension()}

        -   #### getSharedLibraryExtension

            ``` methodSignature
            String getSharedLibraryExtension()
            ```

        []{#getSharedLibraryVersionedExtensionFormat()}

        -   #### getSharedLibraryVersionedExtensionFormat

            ``` methodSignature
            String getSharedLibraryVersionedExtensionFormat()
            ```

        []{#getStaticLibraryExtension()}

        -   #### getStaticLibraryExtension

            ``` methodSignature
            String getStaticLibraryExtension()
            ```

        []{#getObjectFileExtension()}

        -   #### getObjectFileExtension

            ``` methodSignature
            String getObjectFileExtension()
            ```

        []{#getCompilerDebugPathSanitizer()}

        -   #### getCompilerDebugPathSanitizer

            ``` methodSignature
            DebugPathSanitizer getCompilerDebugPathSanitizer()
            ```

        []{#getHeaderVerification()}

        -   #### getHeaderVerification

            ``` methodSignature
            HeaderVerification getHeaderVerification()
            ```

        []{#getUseArgFile()}

        -   #### getUseArgFile

            ``` methodSignature
            Optional<Boolean> getUseArgFile()
            ```

        []{#getFlagMacros()}

        -   #### getFlagMacros

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getFlagMacros()
            ```

            [Returns:]{.returnLabel}
            :   a map for macro names to their respective expansions, to
                be used to expand macro references in user-provided
                flags.

        []{#getSharedLibraryInterfaceParams()}

        -   #### getSharedLibraryInterfaceParams

            ``` methodSignature
            Optional<SharedLibraryInterfaceParams> getSharedLibraryInterfaceParams()
            ```

            [Returns:]{.returnLabel}
            :   params used to determine which shared library interfaces
                to generate, which are used for linking in liu of the
                original shared library.

        []{#getBinaryExtension()}

        -   #### getBinaryExtension

            ``` methodSignature
            Optional<String> getBinaryExtension()
            ```

        []{#getPublicHeadersSymlinksEnabled()}

        -   #### getPublicHeadersSymlinksEnabled

            ``` methodSignature
            boolean getPublicHeadersSymlinksEnabled()
            ```

            ::: block
            When building or creating a project, create symlinks for the
            public headers if it\'s true. It would allow public headers
            to include an other public header with #include
            \"foobar.h\"\\ even if it\'s not in the same folder.
            :::

        []{#getPrivateHeadersSymlinksEnabled()}

        -   #### getPrivateHeadersSymlinksEnabled

            ``` methodSignature
            boolean getPrivateHeadersSymlinksEnabled()
            ```

            ::: block
            When building or creating a project, create symlinks for the
            public headers if it\'s true.
            :::

        []{#getPicTypeForSharedLinking()}

        -   #### getPicTypeForSharedLinking

            ``` methodSignature
            @Default
            default PicType getPicTypeForSharedLinking()
            ```

            ::: block
            nix platforms use PIC object files for shared libraries,
            while windows doesn\'t.
            :::

        []{#getConflictingHeaderBasenameWhitelist()}

        -   #### getConflictingHeaderBasenameWhitelist

            ``` methodSignature
            @Default
            default com.google.common.collect.ImmutableSortedSet<String> getConflictingHeaderBasenameWhitelist()
            ```

            [Returns:]{.returnLabel}
            :   whitelist of basenames to exclude from conflicting
                header checks.

        []{#getHeaderMode()}

        -   #### getHeaderMode

            ``` methodSignature
            Optional<HeaderMode> getHeaderMode()
            ```

            [Returns:]{.returnLabel}
            :   the explicit header mode to use for this platform.

        []{#getFilepathLengthLimited()}

        -   #### getFilepathLengthLimited

            ``` methodSignature
            @Default
            default boolean getFilepathLengthLimited()
            ```

            [Returns:]{.returnLabel}
            :   whether shorter names for intermediate files should be
                used

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static CxxPlatform.Builder builder()
            ```

        []{#withFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### withFlavor

            ``` methodSignature
            default CxxPlatform withFlavor​(Flavor flavor)
            ```

        []{#withAsflags(com.google.common.collect.ImmutableList)}

        -   #### withAsflags

            ``` methodSignature
            default CxxPlatform withAsflags​(com.google.common.collect.ImmutableList<Arg> asFlags)
            ```

        []{#withCppflags(com.google.common.collect.ImmutableList)}

        -   #### withCppflags

            ``` methodSignature
            default CxxPlatform withCppflags​(com.google.common.collect.ImmutableList<Arg> cppFlags)
            ```

        []{#withCflags(com.google.common.collect.ImmutableList)}

        -   #### withCflags

            ``` methodSignature
            default CxxPlatform withCflags​(com.google.common.collect.ImmutableList<Arg> cFlags)
            ```

        []{#withCpp(com.facebook.buck.cxx.toolchain.PreprocessorProvider)}

        -   #### withCpp

            ``` methodSignature
            default CxxPlatform withCpp​(PreprocessorProvider cpp)
            ```

        []{#withConflictingHeaderBasenameWhitelist(com.google.common.collect.ImmutableSortedSet)}

        -   #### withConflictingHeaderBasenameWhitelist

            ``` methodSignature
            default CxxPlatform withConflictingHeaderBasenameWhitelist​(com.google.common.collect.ImmutableSortedSet<String> conflictingHeaderBasenameWhitelist)
            ```

        []{#withCxxppflags(com.google.common.collect.ImmutableList)}

        -   #### withCxxppflags

            ``` methodSignature
            default CxxPlatform withCxxppflags​(com.google.common.collect.ImmutableList<Arg> cxxppflags)
            ```

        []{#withCxxflags(com.google.common.collect.ImmutableList)}

        -   #### withCxxflags

            ``` methodSignature
            default CxxPlatform withCxxflags​(com.google.common.collect.ImmutableList<Arg> cxxFlags)
            ```

        []{#withArchiveContents(com.facebook.buck.cxx.toolchain.ArchiveContents)}

        -   #### withArchiveContents

            ``` methodSignature
            default CxxPlatform withArchiveContents​(ArchiveContents archiveContents)
            ```

        []{#withFlagMacros(com.google.common.collect.ImmutableMap)}

        -   #### withFlagMacros

            ``` methodSignature
            default CxxPlatform withFlagMacros​(com.google.common.collect.ImmutableMap<String,​String> flagMacros)
            ```

        []{#withCompilerDebugPathSanitizer(com.facebook.buck.cxx.toolchain.DebugPathSanitizer)}

        -   #### withCompilerDebugPathSanitizer

            ``` methodSignature
            default CxxPlatform withCompilerDebugPathSanitizer​(DebugPathSanitizer compilerDebugPathSanitizer)
            ```

        []{#withCxxpp(com.facebook.buck.cxx.toolchain.PreprocessorProvider)}

        -   #### withCxxpp

            ``` methodSignature
            default CxxPlatform withCxxpp​(PreprocessorProvider preprocessorProvider)
            ```

        []{#withCxx(com.facebook.buck.cxx.toolchain.CompilerProvider)}

        -   #### withCxx

            ``` methodSignature
            default CxxPlatform withCxx​(CompilerProvider compilerProvider)
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
