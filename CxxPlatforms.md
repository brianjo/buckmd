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
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.impl](package-summary.html)
:::

## Class CxxPlatforms {#class-cxxplatforms .title title="Class CxxPlatforms"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.impl.CxxPlatforms

::: description
-   

    ------------------------------------------------------------------------

        public class CxxPlatforms
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `addToolFlags         |                       |
        |                       | FromConfig​(CxxBuckCon |                       |
        |                       | fig config,           |                       |
        |                       |              CxxPlatf |                       |
        |                       | orm.Builder builder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CxxPlatform`  | `build​(Flavor         |                       |
        |                       |  flavor,      Platfor |                       |
        |                       | m platform,      CxxB |                       |
        |                       | uckConfig config,     |                       |
        |                       |   CompilerProvider as |                       |
        |                       | ,      PreprocessorPr |                       |
        |                       | ovider aspp,      Com |                       |
        |                       | pilerProvider cc,     |                       |
        |                       |   CompilerProvider cx |                       |
        |                       | x,      PreprocessorP |                       |
        |                       | rovider cpp,      Pre |                       |
        |                       | processorProvider cxx |                       |
        |                       | pp,      LinkerProvid |                       |
        |                       | er ld,      Iterable< |                       |
        |                       | Arg> ldFlags,      co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableMultimap< |                       |
        |                       | Linker.LinkableDepTyp |                       |
        |                       | e,​Arg> runtimeLdflags |                       |
        |                       | ,      Tool strip,    |                       |
        |                       |    ArchiverProvider a |                       |
        |                       | r,      ArchiveConten |                       |
        |                       | ts archiveContents,   |                       |
        |                       |     Optional<ToolProv |                       |
        |                       | ider> ranlib,      Sy |                       |
        |                       | mbolNameTool nm,      |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList<A |                       |
        |                       | rg> asflags,      com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Arg>  |                       |
        |                       | asppflags,      com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList<Arg> cf |                       |
        |                       | lags,      com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableList<Arg> cppflag |                       |
        |                       | s,      com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<Arg> cxxflags,  |                       |
        |                       |      com.google.commo |                       |
        |                       | n.collect.ImmutableLi |                       |
        |                       | st<Arg> cxxppflags,   |                       |
        |                       |     String sharedLibr |                       |
        |                       | aryExtension,      St |                       |
        |                       | ring sharedLibraryVer |                       |
        |                       | sionedExtensionFormat |                       |
        |                       | ,      String staticL |                       |
        |                       | ibraryExtension,      |                       |
        |                       |  String objectFileExt |                       |
        |                       | ension,      Optional |                       |
        |                       | <SharedLibraryInterfa |                       |
        |                       | ceParams> defaultShar |                       |
        |                       | edLibraryInterfacePar |                       |
        |                       | ams,      DebugPathSa |                       |
        |                       | nitizer compilerDebug |                       |
        |                       | PathSanitizer,      c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableMap<Stri |                       |
        |                       | ng,​String> flagMacros |                       |
        |                       | ,      Optional<Strin |                       |
        |                       | g> binaryExtension,   |                       |
        |                       |     HeaderVerificatio |                       |
        |                       | n headerVerification, |                       |
        |                       |       boolean publicH |                       |
        |                       | eadersSymlinksEnabled |                       |
        |                       | ,      boolean privat |                       |
        |                       | eHeadersSymlinksEnabl |                       |
        |                       | ed,      PicType picT |                       |
        |                       | ypeForSharedLinking)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CxxPlatform`  | `                     | ::: block             |
        |                       | copyPlatformWithFlavo | Creates a CxxPlatform |
        |                       | rAndConfig​(CxxPlatfor | with a defined flavor |
        |                       | m defaultPlatform,    | for a CxxBuckConfig   |
        |                       |                       | with default values   |
        |                       |         Platform plat | provided from another |
        |                       | form,                 | default CxxPlatform   |
        |                       |                 CxxBu | :::                   |
        |                       | ckConfig config,      |                       |
        |                       |                       |                       |
        |                       |       Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static I             | `findDepsFo           |                       |
        | terable<BuildTarget>` | rTargetFromConstructo |                       |
        |                       | rArgs​(CxxPlatformsPro |                       |
        |                       | vider cxxPlatformsPro |                       |
        |                       | vider,                |                       |
        |                       |                       |                       |
        |                       |  BuildTarget buildTar |                       |
        |                       | get,                  |                       |
        |                       |                     O |                       |
        |                       | ptional<Flavor> defau |                       |
        |                       | ltCxxPlatformFlavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `getAllP              |                       |
        | oogle.common.collect. | ossibleHostFlavors()` |                       |
        | ImmutableSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static U             | `getConfigDefau       | ::: block             |
        | nresolvedCxxPlatform` | ltCxxPlatform​(CxxBuck | Returns the           |
        |                       | Config cxxBuckConfig, | configured default    |
        |                       |                       | cxx platform.         |
        |                       |        com.google.com | :::                   |
        |                       | mon.collect.Immutable |                       |
        |                       | Map<Flavor,​Unresolved |                       |
        |                       | CxxPlatform> cxxPlatf |                       |
        |                       | ormsMap,              |                       |
        |                       |                Unreso |                       |
        |                       | lvedCxxPlatform syste |                       |
        |                       | mDefaultCxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static U             | `ge                   | ::: block             |
        | nresolvedCxxPlatform` | tCxxPlatform​(CxxPlatf | Returns the           |
        |                       | ormsProvider cxxPlatf | configured cxx        |
        |                       | ormsProvider,         | platform for a        |
        |                       |        BuildTarget ta | particular target.    |
        |                       | rget,               O | :::                   |
        |                       | ptional<Flavor> defau |                       |
        |                       | ltCxxPlatformFlavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Flavor`       | `getHostFlavor()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static I             | `getParseTimeDep      |                       |
        | terable<BuildTarget>` | s​(TargetConfiguration |                       |
        |                       |  targetConfiguration, |                       |
        |                       |                  CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.facebook.buck.core.model.Flavor,com.facebook.buck.util.environment.Platform,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CompilerProvider,com.facebook.buck.cxx.toolchain.PreprocessorProvider,com.facebook.buck.cxx.toolchain.CompilerProvider,com.facebook.buck.cxx.toolchain.CompilerProvider,com.facebook.buck.cxx.toolchain.PreprocessorProvider,com.facebook.buck.cxx.toolchain.PreprocessorProvider,com.facebook.buck.cxx.toolchain.linker.LinkerProvider,java.lang.Iterable,com.google.common.collect.ImmutableMultimap,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.cxx.toolchain.ArchiverProvider,com.facebook.buck.cxx.toolchain.ArchiveContents,java.util.Optional,com.facebook.buck.cxx.toolchain.SymbolNameTool,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.util.Optional,com.facebook.buck.cxx.toolchain.DebugPathSanitizer,com.google.common.collect.ImmutableMap,java.util.Optional,com.facebook.buck.cxx.toolchain.HeaderVerification,boolean,boolean,com.facebook.buck.cxx.toolchain.PicType)}

        -   #### build

            ``` methodSignature
            public static CxxPlatform build​(Flavor flavor,
                                            Platform platform,
                                            CxxBuckConfig config,
                                            CompilerProvider as,
                                            PreprocessorProvider aspp,
                                            CompilerProvider cc,
                                            CompilerProvider cxx,
                                            PreprocessorProvider cpp,
                                            PreprocessorProvider cxxpp,
                                            LinkerProvider ld,
                                            Iterable<Arg> ldFlags,
                                            com.google.common.collect.ImmutableMultimap<Linker.LinkableDepType,​Arg> runtimeLdflags,
                                            Tool strip,
                                            ArchiverProvider ar,
                                            ArchiveContents archiveContents,
                                            Optional<ToolProvider> ranlib,
                                            SymbolNameTool nm,
                                            com.google.common.collect.ImmutableList<Arg> asflags,
                                            com.google.common.collect.ImmutableList<Arg> asppflags,
                                            com.google.common.collect.ImmutableList<Arg> cflags,
                                            com.google.common.collect.ImmutableList<Arg> cppflags,
                                            com.google.common.collect.ImmutableList<Arg> cxxflags,
                                            com.google.common.collect.ImmutableList<Arg> cxxppflags,
                                            String sharedLibraryExtension,
                                            String sharedLibraryVersionedExtensionFormat,
                                            String staticLibraryExtension,
                                            String objectFileExtension,
                                            Optional<SharedLibraryInterfaceParams> defaultSharedLibraryInterfaceParams,
                                            DebugPathSanitizer compilerDebugPathSanitizer,
                                            com.google.common.collect.ImmutableMap<String,​String> flagMacros,
                                            Optional<String> binaryExtension,
                                            HeaderVerification headerVerification,
                                            boolean publicHeadersSymlinksEnabled,
                                            boolean privateHeadersSymlinksEnabled,
                                            PicType picTypeForSharedLinking)
            ```

        []{#copyPlatformWithFlavorAndConfig(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.util.environment.Platform,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.core.model.Flavor)}

        -   #### copyPlatformWithFlavorAndConfig

            ``` methodSignature
            public static CxxPlatform copyPlatformWithFlavorAndConfig​(CxxPlatform defaultPlatform,
                                                                      Platform platform,
                                                                      CxxBuckConfig config,
                                                                      Flavor flavor)
            ```

            ::: block
            Creates a CxxPlatform with a defined flavor for a
            CxxBuckConfig with default values provided from another
            default CxxPlatform
            :::

        []{#getAllPossibleHostFlavors()}

        -   #### getAllPossibleHostFlavors

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Flavor> getAllPossibleHostFlavors()
            ```

        []{#getHostFlavor()}

        -   #### getHostFlavor

            ``` methodSignature
            public static Flavor getHostFlavor()
            ```

        []{#addToolFlagsFromConfig(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform.Builder)}

        -   #### addToolFlagsFromConfig

            ``` methodSignature
            public static void addToolFlagsFromConfig​(CxxBuckConfig config,
                                                      CxxPlatform.Builder builder)
            ```

        []{#getConfigDefaultCxxPlatform(com.facebook.buck.cxx.config.CxxBuckConfig,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.UnresolvedCxxPlatform)}

        -   #### getConfigDefaultCxxPlatform

            ``` methodSignature
            public static UnresolvedCxxPlatform getConfigDefaultCxxPlatform​(CxxBuckConfig cxxBuckConfig,
                                                                            com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform> cxxPlatformsMap,
                                                                            UnresolvedCxxPlatform systemDefaultCxxPlatform)
            ```

            ::: block
            Returns the configured default cxx platform.
            :::

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public static Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration,
                                                                 CxxPlatform cxxPlatform)
            ```

        []{#getCxxPlatform(com.facebook.buck.cxx.toolchain.CxxPlatformsProvider,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### getCxxPlatform

            ``` methodSignature
            public static UnresolvedCxxPlatform getCxxPlatform​(CxxPlatformsProvider cxxPlatformsProvider,
                                                               BuildTarget target,
                                                               Optional<Flavor> defaultCxxPlatformFlavor)
            ```

            ::: block
            Returns the configured cxx platform for a particular target.
            :::

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.cxx.toolchain.CxxPlatformsProvider,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public static Iterable<BuildTarget> findDepsForTargetFromConstructorArgs​(CxxPlatformsProvider cxxPlatformsProvider,
                                                                                     BuildTarget buildTarget,
                                                                                     Optional<Flavor> defaultCxxPlatformFlavor)
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
-   Nested \| 
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
