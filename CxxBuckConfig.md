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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.config](package-summary.html)
:::

## Class CxxBuckConfig {#class-cxxbuckconfig .title title="Class CxxBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.config.CxxBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class CxxBuckConfig
        extends Object

    ::: block
    Contains platform independent settings for C/C++ rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                           Description
          ------------------- ------------------------------- -------------
          `static String`     `DEFAULT_FLAVOR_LIBRARY_TYPE`    
          `static String`     `DEFAULT_FLAVOR_PLATFORM`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                        Description
          ------------------------------------------------------------------ -------------
          `CxxBuckConfig​(BuckConfig delegate)`                                
          `CxxBuckConfig​(BuckConfig delegate,              Flavor flavor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `                     |                       |
        |                       | checkGTestTestList()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `                     |                       |
        | nal<ArchiveContents>` | getArchiveContents()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getA                 |                       |
        | al<ArchiverProvider>` | rchiverProvider​(Platf |                       |
        |                       | orm defaultPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getArflags()`        |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getAs()`             |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getAsflags()`        |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getAsm()`            |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getAsmflags()`       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getAsmpp()`          |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getAsmppflags()`     |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getAspp()`           |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getAsppflags()`      |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getBinaryExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getBoostTestDep      |                       |
        | ptional<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCc()`             |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCflags()`         |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getConflictingHeade  |                       |
        | common.collect.Immuta | rBasenameWhitelist()` |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getCpp()`            |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCppflags()`       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCuda()`           |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCudaflags()`      |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getCudapp()`         |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCudappflags()`    |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCxx()`            |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCxxflags()`       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `getCxxFlavor         | ::: block             |
        | oogle.common.collect. | s​(BuckConfig config)` | Constructs set of     |
        | ImmutableSet<Flavor>` |                       | flavors given in a    |
        |                       |                       | .buckconfig file, as  |
        |                       |                       | is specified by       |
        |                       |                       | section names of the  |
        |                       |                       | form cxx#{flavor      |
        |                       |                       | name}.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getCxxpp()`          |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getCxxppflags()`     |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getDebug             |                       |
        |                       | PathSanitizerLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `ge                   |                       |
        | oogle.common.collect. | tDeclaredPlatforms()` |                       |
        | ImmutableSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `ge                   |                       |
        | ommon.collect.Immutab | tDefaultFlavorsForRul |                       |
        | leMap<String,​Flavor>` | eType​(RuleType type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getDefaultPlatform()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | getDefaultReexportAll |                       |
        |                       | HeaderDependencies()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEnvironment()`    |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `getFil               |                       |
        |                       | epathLengthLimited()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `                     |                       |
        | ollect.ImmutableMap<F | getFlavoredConfigs()` |                       |
        | lavor,​CxxBuckConfig>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getGt                |                       |
        | ptional<BuildTarget>` | estDefaultTestMainDep |                       |
        |                       | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getGtestDep          |                       |
        | ptional<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getHeaderMode()`     |                       |
        | Optional<HeaderMode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HeaderVerification`  | `getHeaderVe          |                       |
        |                       | rificationOrIgnore()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getHip()`            |                       |
        | al<CompilerProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getHipflags()`       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<P           | `getHippp()`          |                       |
        | reprocessorProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getHipppflags()`     |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getHostPlatform()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getIndependentShli   |                       |
        | gle.common.collect.Im | bInterfacesLdflags()` |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getLdflags()`        |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `getLinker            | ::: block             |
        | onal<LinkerProvider>` | Provider​(LinkerProvid | Construct a linker    |
        |                       | er.Type defaultType)` | based on \`ld\` and   |
        |                       |                       | \`linker_platform\`   |
        |                       |                       | sections in the       |
        |                       |                       | config.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `ge                   |                       |
        |                       | tLinkGroupsEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getLinkGr            |                       |
        |                       | oupsEnabledSetting()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `g                    |                       |
        | al<RuleScheduleInfo>` | etLinkScheduleInfo()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getMax               |                       |
        |                       | imumTestOutputSize()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getNm()`             |                       |
        | tional<ToolProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getObjcopy()`        |                       |
        | tional<ToolProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getO                 |                       |
        |                       | bjectFileExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `                     |                       |
        |                       | getPath​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getPrivateHead       |                       |
        |                       | ersSymlinksEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getPrivateHead       |                       |
        |                       | ersSymlinksSetting()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional<Un   | `getProviderBasedPlat | ::: block             |
        | resolvedCxxPlatform>` | form​(BuckConfig confi | If the config         |
        |                       | g,                    | specifies a value for |
        |                       |       Flavor flavor)` | \"toolchain_target\", |
        |                       |                       | returns a             |
        |                       |                       | [`Unreso              |
        |                       |                       | lvedCxxPlatform`](../ |
        |                       |                       | toolchain/UnresolvedC |
        |                       |                       | xxPlatform.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |                       | backed by the         |
        |                       |                       | specified target.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getPublicHead        |                       |
        |                       | ersSymlinksEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getPublicHead        |                       |
        |                       | ersSymlinksSetting()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getRanlib()`         |                       |
        | tional<ToolProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getRanlibflags()`    |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getShar              |                       |
        |                       | edLibraryExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getShare             |                       |
        | tional<SharedLibraryI | dLibraryInterfaces()` |                       |
        | nterfaceParams.Type>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getShoul             |                       |
        |                       | dRemapHostPlatform()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSourcePath​(Stri   |                       |
        | Optional<SourcePath>` | ng name,              |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PathSourcePath`      | `getS                 |                       |
        |                       | ourcePath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getStat              |                       |
        |                       | icLibraryExtension()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Tool>`      | `getStrip()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getUseArgFile()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `getUseDetailedUntra  |                       |
        |                       | ckedHeaderMessages()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isIndependentShare   |                       |
        |                       | dLibraryInterfaces()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPCHEnabled()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isUnique             |                       |
        |                       | LibraryNameEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `s                    |                       |
        |                       | houldCacheBinaries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldCacheLinks()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldCacheStrip()`  |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_FLAVOR_LIBRARY_TYPE}

        -   #### DEFAULT_FLAVOR_LIBRARY_TYPE

                public static final String DEFAULT_FLAVOR_LIBRARY_TYPE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.cxx.config.CxxBuckConfig.DEFAULT_FLAVOR_LIBRARY_TYPE)

        []{#DEFAULT_FLAVOR_PLATFORM}

        -   #### DEFAULT_FLAVOR_PLATFORM

                public static final String DEFAULT_FLAVOR_PLATFORM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.cxx.config.CxxBuckConfig.DEFAULT_FLAVOR_PLATFORM)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### CxxBuckConfig

                public CxxBuckConfig​(BuckConfig delegate)

        []{#<init>(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.model.Flavor)}

        -   #### CxxBuckConfig

                public CxxBuckConfig​(BuckConfig delegate,
                                     Flavor flavor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCxxFlavors(com.facebook.buck.core.config.BuckConfig)}

        -   #### getCxxFlavors

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Flavor> getCxxFlavors​(BuckConfig config)
            ```

            ::: block
            Constructs set of flavors given in a .buckconfig file, as is
            specified by section names of the form cxx#{flavor name}.
            :::

        []{#getFlavoredConfigs()}

        -   #### getFlavoredConfigs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Flavor,​CxxBuckConfig> getFlavoredConfigs()
            ```

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

            [Returns:]{.returnLabel}
            :   the environment in which
                [`BuckConfig`](../../core/config/BuckConfig.html "class in com.facebook.buck.core.config")
                was created.

        []{#getGtestDep(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getGtestDep

            ``` methodSignature
            public Optional<BuildTarget> getGtestDep​(TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                which represents the gtest library.

        []{#getGtestDefaultTestMainDep(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getGtestDefaultTestMainDep

            ``` methodSignature
            public Optional<BuildTarget> getGtestDefaultTestMainDep​(TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                which represents the main function that gtest tests
                should use by default (if no other main is given).

        []{#getBoostTestDep(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getBoostTestDep

            ``` methodSignature
            public Optional<BuildTarget> getBoostTestDep​(TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                which represents the boost testing library.

        []{#getPath(java.lang.String)}

        -   #### getPath

            ``` methodSignature
            public Optional<Path> getPath​(String name)
            ```

        []{#getSourcePath(java.nio.file.Path)}

        -   #### getSourcePath

            ``` methodSignature
            @Nullable
            public PathSourcePath getSourcePath​(Path path)
            ```

        []{#getSourcePath(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getSourcePath

            ``` methodSignature
            public Optional<SourcePath> getSourcePath​(String name,
                                                      TargetConfiguration targetConfiguration)
            ```

        []{#getDefaultPlatform()}

        -   #### getDefaultPlatform

            ``` methodSignature
            public Optional<String> getDefaultPlatform()
            ```

        []{#getHostPlatform()}

        -   #### getHostPlatform

            ``` methodSignature
            public Optional<String> getHostPlatform()
            ```

        []{#getAsflags()}

        -   #### getAsflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getAsflags()
            ```

        []{#getAsppflags()}

        -   #### getAsppflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getAsppflags()
            ```

        []{#getCflags()}

        -   #### getCflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCflags()
            ```

        []{#getCxxflags()}

        -   #### getCxxflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCxxflags()
            ```

        []{#getCppflags()}

        -   #### getCppflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCppflags()
            ```

        []{#getCxxppflags()}

        -   #### getCxxppflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCxxppflags()
            ```

        []{#getCudaflags()}

        -   #### getCudaflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCudaflags()
            ```

        []{#getCudappflags()}

        -   #### getCudappflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCudappflags()
            ```

        []{#getHipflags()}

        -   #### getHipflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getHipflags()
            ```

        []{#getHipppflags()}

        -   #### getHipppflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getHipppflags()
            ```

        []{#getAsmflags()}

        -   #### getAsmflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getAsmflags()
            ```

        []{#getAsmppflags()}

        -   #### getAsmppflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getAsmppflags()
            ```

        []{#getLdflags()}

        -   #### getLdflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getLdflags()
            ```

        []{#getArflags()}

        -   #### getArflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getArflags()
            ```

        []{#getRanlibflags()}

        -   #### getRanlibflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getRanlibflags()
            ```

        []{#getArchiverProvider(com.facebook.buck.util.environment.Platform)}

        -   #### getArchiverProvider

            ``` methodSignature
            public Optional<ArchiverProvider> getArchiverProvider​(Platform defaultPlatform)
            ```

        []{#getMaximumTestOutputSize()}

        -   #### getMaximumTestOutputSize

            ``` methodSignature
            public long getMaximumTestOutputSize()
            ```

            [Returns:]{.returnLabel}
            :   the maximum size in bytes of test output to report in
                test results.

        []{#getAs()}

        -   #### getAs

            ``` methodSignature
            public Optional<CompilerProvider> getAs()
            ```

        []{#getAspp()}

        -   #### getAspp

            ``` methodSignature
            public Optional<PreprocessorProvider> getAspp()
            ```

        []{#getCc()}

        -   #### getCc

            ``` methodSignature
            public Optional<CompilerProvider> getCc()
            ```

        []{#getCpp()}

        -   #### getCpp

            ``` methodSignature
            public Optional<PreprocessorProvider> getCpp()
            ```

        []{#getCxx()}

        -   #### getCxx

            ``` methodSignature
            public Optional<CompilerProvider> getCxx()
            ```

        []{#getCxxpp()}

        -   #### getCxxpp

            ``` methodSignature
            public Optional<PreprocessorProvider> getCxxpp()
            ```

        []{#getCuda()}

        -   #### getCuda

            ``` methodSignature
            public Optional<CompilerProvider> getCuda()
            ```

        []{#getCudapp()}

        -   #### getCudapp

            ``` methodSignature
            public Optional<PreprocessorProvider> getCudapp()
            ```

        []{#getHip()}

        -   #### getHip

            ``` methodSignature
            public Optional<CompilerProvider> getHip()
            ```

        []{#getHippp()}

        -   #### getHippp

            ``` methodSignature
            public Optional<PreprocessorProvider> getHippp()
            ```

        []{#getAsm()}

        -   #### getAsm

            ``` methodSignature
            public Optional<CompilerProvider> getAsm()
            ```

        []{#getAsmpp()}

        -   #### getAsmpp

            ``` methodSignature
            public Optional<PreprocessorProvider> getAsmpp()
            ```

        []{#getUseArgFile()}

        -   #### getUseArgFile

            ``` methodSignature
            public Optional<Boolean> getUseArgFile()
            ```

        []{#getLinkerProvider(com.facebook.buck.cxx.toolchain.linker.LinkerProvider.Type)}

        -   #### getLinkerProvider

            ``` methodSignature
            public Optional<LinkerProvider> getLinkerProvider​(LinkerProvider.Type defaultType)
            ```

            ::: block
            Construct a linker based on \`ld\` and \`linker_platform\`
            sections in the config.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultType` - the default type for a linker if
                \`linker_platform\` is not specified in the config.

        []{#getHeaderVerificationOrIgnore()}

        -   #### getHeaderVerificationOrIgnore

            ``` methodSignature
            public HeaderVerification getHeaderVerificationOrIgnore()
            ```

        []{#getLinkGroupsEnabledSetting()}

        -   #### getLinkGroupsEnabledSetting

            ``` methodSignature
            public Optional<Boolean> getLinkGroupsEnabledSetting()
            ```

        []{#getLinkGroupsEnabled()}

        -   #### getLinkGroupsEnabled

            ``` methodSignature
            public boolean getLinkGroupsEnabled()
            ```

        []{#getPublicHeadersSymlinksSetting()}

        -   #### getPublicHeadersSymlinksSetting

            ``` methodSignature
            public Optional<Boolean> getPublicHeadersSymlinksSetting()
            ```

        []{#getPublicHeadersSymlinksEnabled()}

        -   #### getPublicHeadersSymlinksEnabled

            ``` methodSignature
            public boolean getPublicHeadersSymlinksEnabled()
            ```

        []{#getPrivateHeadersSymlinksSetting()}

        -   #### getPrivateHeadersSymlinksSetting

            ``` methodSignature
            public Optional<Boolean> getPrivateHeadersSymlinksSetting()
            ```

        []{#getPrivateHeadersSymlinksEnabled()}

        -   #### getPrivateHeadersSymlinksEnabled

            ``` methodSignature
            public boolean getPrivateHeadersSymlinksEnabled()
            ```

        []{#getLinkScheduleInfo()}

        -   #### getLinkScheduleInfo

            ``` methodSignature
            public Optional<RuleScheduleInfo> getLinkScheduleInfo()
            ```

        []{#shouldCacheLinks()}

        -   #### shouldCacheLinks

            ``` methodSignature
            public boolean shouldCacheLinks()
            ```

        []{#shouldCacheStrip()}

        -   #### shouldCacheStrip

            ``` methodSignature
            public boolean shouldCacheStrip()
            ```

        []{#shouldCacheBinaries()}

        -   #### shouldCacheBinaries

            ``` methodSignature
            public boolean shouldCacheBinaries()
            ```

        []{#checkGTestTestList()}

        -   #### checkGTestTestList

            ``` methodSignature
            public boolean checkGTestTestList()
            ```

        []{#isPCHEnabled()}

        -   #### isPCHEnabled

            ``` methodSignature
            public boolean isPCHEnabled()
            ```

        []{#getArchiveContents()}

        -   #### getArchiveContents

            ``` methodSignature
            public Optional<ArchiveContents> getArchiveContents()
            ```

        []{#getDefaultFlavorsForRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### getDefaultFlavorsForRuleType

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​Flavor> getDefaultFlavorsForRuleType​(RuleType type)
            ```

        []{#getDebugPathSanitizerLimit()}

        -   #### getDebugPathSanitizerLimit

            ``` methodSignature
            public int getDebugPathSanitizerLimit()
            ```

        []{#getShouldRemapHostPlatform()}

        -   #### getShouldRemapHostPlatform

            ``` methodSignature
            public boolean getShouldRemapHostPlatform()
            ```

            [Returns:]{.returnLabel}
            :   whether to remap to the underlying host platform or to
                use #default

        []{#getRanlib()}

        -   #### getRanlib

            ``` methodSignature
            public Optional<ToolProvider> getRanlib()
            ```

        []{#getObjcopy()}

        -   #### getObjcopy

            ``` methodSignature
            public Optional<ToolProvider> getObjcopy()
            ```

        []{#getNm()}

        -   #### getNm

            ``` methodSignature
            public Optional<ToolProvider> getNm()
            ```

        []{#getStrip()}

        -   #### getStrip

            ``` methodSignature
            public Optional<Tool> getStrip()
            ```

        []{#isUniqueLibraryNameEnabled()}

        -   #### isUniqueLibraryNameEnabled

            ``` methodSignature
            public boolean isUniqueLibraryNameEnabled()
            ```

        []{#getDefaultReexportAllHeaderDependencies()}

        -   #### getDefaultReexportAllHeaderDependencies

            ``` methodSignature
            public boolean getDefaultReexportAllHeaderDependencies()
            ```

        []{#getSharedLibraryInterfaces()}

        -   #### getSharedLibraryInterfaces

            ``` methodSignature
            public Optional<SharedLibraryInterfaceParams.Type> getSharedLibraryInterfaces()
            ```

            [Returns:]{.returnLabel}
            :   whether to enable shared library interfaces.

        []{#getIndependentShlibInterfacesLdflags()}

        -   #### getIndependentShlibInterfacesLdflags

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getIndependentShlibInterfacesLdflags()
            ```

            [Returns:]{.returnLabel}
            :   additional flags to pass to the linker when linking
                independent shared library interfaces.

        []{#isIndependentSharedLibraryInterfaces()}

        -   #### isIndependentSharedLibraryInterfaces

            ``` methodSignature
            public boolean isIndependentSharedLibraryInterfaces()
            ```

            [Returns:]{.returnLabel}
            :   whether to generate a rule\'s shared library interface
                directly from it\'s object files, to avoid having to
                wait for it\'s shared library to build.

        []{#getDeclaredPlatforms()}

        -   #### getDeclaredPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Flavor> getDeclaredPlatforms()
            ```

            [Returns:]{.returnLabel}
            :   the list of flavors that buck will consider valid when
                building the target graph.

        []{#getBinaryExtension()}

        -   #### getBinaryExtension

            ``` methodSignature
            public Optional<String> getBinaryExtension()
            ```

            [Returns:]{.returnLabel}
            :   the extension to use for binaries (e.g. \".exe\").

        []{#getSharedLibraryExtension()}

        -   #### getSharedLibraryExtension

            ``` methodSignature
            public Optional<String> getSharedLibraryExtension()
            ```

            [Returns:]{.returnLabel}
            :   the extension to use for shared libraries (e.g.
                \".so\").

        []{#getStaticLibraryExtension()}

        -   #### getStaticLibraryExtension

            ``` methodSignature
            public Optional<String> getStaticLibraryExtension()
            ```

            [Returns:]{.returnLabel}
            :   the extension to use for static libraries (e.g. \".a\").

        []{#getObjectFileExtension()}

        -   #### getObjectFileExtension

            ``` methodSignature
            public Optional<String> getObjectFileExtension()
            ```

            [Returns:]{.returnLabel}
            :   the extension to use for object files (e.g. \".o\").

        []{#getConflictingHeaderBasenameWhitelist()}

        -   #### getConflictingHeaderBasenameWhitelist

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getConflictingHeaderBasenameWhitelist()
            ```

        []{#getHeaderMode()}

        -   #### getHeaderMode

            ``` methodSignature
            public Optional<HeaderMode> getHeaderMode()
            ```

            [Returns:]{.returnLabel}
            :   the configured C/C++ header mode.

        []{#getUseDetailedUntrackedHeaderMessages()}

        -   #### getUseDetailedUntrackedHeaderMessages

            ``` methodSignature
            public Boolean getUseDetailedUntrackedHeaderMessages()
            ```

            [Returns:]{.returnLabel}
            :   whether to generate more detailed untracked header
                messages.

        []{#getFilepathLengthLimited()}

        -   #### getFilepathLengthLimited

            ``` methodSignature
            public Boolean getFilepathLengthLimited()
            ```

            [Returns:]{.returnLabel}
            :   whether short names for intermediate files should be
                used

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

        []{#getProviderBasedPlatform(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.model.Flavor)}

        -   #### getProviderBasedPlatform

            ``` methodSignature
            public static Optional<UnresolvedCxxPlatform> getProviderBasedPlatform​(BuckConfig config,
                                                                                   Flavor flavor)
            ```

            ::: block
            If the config specifies a value for \"toolchain_target\",
            returns a
            [`UnresolvedCxxPlatform`](../toolchain/UnresolvedCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
            backed by the specified target.
            :::
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
