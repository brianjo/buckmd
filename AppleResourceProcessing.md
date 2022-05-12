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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleResourceProcessing {#class-appleresourceprocessing .title title="Class AppleResourceProcessing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleResourceProcessing

::: description
-   

    ------------------------------------------------------------------------

        public class AppleResourceProcessing
        extends Object

    ::: block
    Contains shared logic for adding resource processing steps to apple
    build rules
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                          Field                 Description
          ---------------------------------------------------------- --------------------- -------------
          `static com.google.common.collect.ImmutableList<String>`   `BASE_IBTOOL_FLAGS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `addFra               | ::: block             |
        |                       | meworksProcessingStep | Adds framework        |
        |                       | s​(Set<SourcePath> fra | processing steps to a |
        |                       | meworks,              | build rule            |
        |                       |                 Path  | :::                   |
        |                       | dirRoot,              |                       |
        |                       |                 com.f |                       |
        |                       | acebook.buck.apple.Ap |                       |
        |                       | pleBundleDestinations |                       |
        |                       |  destinations,        |                       |
        |                       |                       |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList.B |                       |
        |                       | uilder<Step> stepsBui |                       |
        |                       | lder,                 |                       |
        |                       |              BuildCon |                       |
        |                       | text context,         |                       |
        |                       |                       |                       |
        |                       | ProjectFilesystem pro |                       |
        |                       | jectFilesystem,       |                       |
        |                       |                       |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<Path> codeSig |                       |
        |                       | nOnCopyPathsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `                     | ::: block             |
        |                       | addResourceProcessing | Adds Resources        |
        |                       | Steps​(SourcePathResol | processing steps to a |
        |                       | verAdapter resolver,  | build rule            |
        |                       |                       | :::                   |
        |                       |      Path sourcePath, |                       |
        |                       |                       |                       |
        |                       |       Path destinatio |                       |
        |                       | nPath,                |                       |
        |                       |             com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableList.Builder<Ste |                       |
        |                       | p> stepsBuilder,      |                       |
        |                       |                       |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList<S |                       |
        |                       | tring> ibtoolFlags,   |                       |
        |                       |                       |                       |
        |                       |     ProjectFilesystem |                       |
        |                       |  projectFilesystem,   |                       |
        |                       |                       |                       |
        |                       |     boolean isLegacyW |                       |
        |                       | atchApp,              |                       |
        |                       |               ApplePl |                       |
        |                       | atform platform,      |                       |
        |                       |                       |                       |
        |                       |  Logger LOG,          |                       |
        |                       |                   Too |                       |
        |                       | l ibtool,             |                       |
        |                       |                boolea |                       |
        |                       | n ibtoolModuleFlag,   |                       |
        |                       |                       |                       |
        |                       |     BuildTarget build |                       |
        |                       | Target,               |                       |
        |                       |              Optional |                       |
        |                       | <String> binaryName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `add                  | ::: block             |
        |                       | StepsToCopyResources​( | Adds required copy    |
        |                       | BuildContext context, | resources steps       |
        |                       |                       | :::                   |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | .Builder<Step> stepsB |                       |
        |                       | uilder,               |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleList.Builder<Path> |                       |
        |                       |  codeSignOnCopyPathsB |                       |
        |                       | uilder,               |                       |
        |                       |           AppleBundle |                       |
        |                       | Resources resources,  |                       |
        |                       |                       |                       |
        |                       |   boolean verifyResou |                       |
        |                       | rces,                 |                       |
        |                       |         Path dirRoot, |                       |
        |                       |                       |                       |
        |                       |    com.facebook.buck. |                       |
        |                       | apple.AppleBundleDest |                       |
        |                       | inations destinations |                       |
        |                       | ,                     |                       |
        |                       |     ProjectFilesystem |                       |
        |                       |  projectFilesystem,   |                       |
        |                       |                       |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList<S |                       |
        |                       | tring> ibtoolFlags,   |                       |
        |                       |                       |                       |
        |                       |  boolean isLegacyWatc |                       |
        |                       | hApp,                 |                       |
        |                       |         ApplePlatform |                       |
        |                       |  platform,            |                       |
        |                       |              Logger L |                       |
        |                       | OG,                   |                       |
        |                       |       Tool ibtool,    |                       |
        |                       |                       |                       |
        |                       | boolean ibtoolModuleF |                       |
        |                       | lag,                  |                       |
        |                       |        BuildTarget bu |                       |
        |                       | ildTarget,            |                       |
        |                       |              Optional |                       |
        |                       | <String> binaryName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `addSt                | ::: block             |
        |                       | oryboardProcessingSte | Add Storyboard        |
        |                       | ps​(SourcePathResolver | processing ibtool     |
        |                       | Adapter resolver,     | steps to a build rule |
        |                       |                       | :::                   |
        |                       |     Path sourcePath,  |                       |
        |                       |                       |                       |
        |                       |        Path destinati |                       |
        |                       | onPath,               |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList.Builder< |                       |
        |                       | Step> stepsBuilder,   |                       |
        |                       |                       |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist<String> ibtoolFla |                       |
        |                       | gs,                   |                       |
        |                       |            boolean is |                       |
        |                       | LegacyWatchApp,       |                       |
        |                       |                       |                       |
        |                       |   ApplePlatform platf |                       |
        |                       | orm,                  |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem projectFiles |                       |
        |                       | ystem,                |                       |
        |                       |               Logger  |                       |
        |                       | LOG,                  |                       |
        |                       |             Tool ibto |                       |
        |                       | ol,                   |                       |
        |                       |            boolean ib |                       |
        |                       | toolModuleFlag,       |                       |
        |                       |                       |                       |
        |                       |   BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |              Optional |                       |
        |                       | <String> binaryName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `addSwiftSt           | ::: block             |
        |                       | dlibStepIfNeeded​(Sour | Adds the swift stdlib |
        |                       | cePathResolverAdapter | to the bundle if      |
        |                       |  resolver,            | needed                |
        |                       |                 Path  | :::                   |
        |                       | destinationPath,      |                       |
        |                       |                       |                       |
        |                       |  Path bundleRoot,     |                       |
        |                       |                       |                       |
        |                       |   Optional<java.util. |                       |
        |                       | function.Supplier<Cod |                       |
        |                       | eSignIdentity>> codeS |                       |
        |                       | ignIdentitySupplier,  |                       |
        |                       |                       |                       |
        |                       |      com.google.commo |                       |
        |                       | n.collect.ImmutableLi |                       |
        |                       | st.Builder<Step> step |                       |
        |                       | sBuilder,             |                       |
        |                       |                boolea |                       |
        |                       | n isForPackaging,     |                       |
        |                       |                       |                       |
        |                       |   String bundleExtens |                       |
        |                       | ion,                  |                       |
        |                       |           boolean cop |                       |
        |                       | ySwiftStdlibToFramewo |                       |
        |                       | rks,                  |                       |
        |                       |           boolean use |                       |
        |                       | LipoThin,             |                       |
        |                       |                Option |                       |
        |                       | al<Tool> swiftStdlibT |                       |
        |                       | ool,                  |                       |
        |                       |           ProjectFile |                       |
        |                       | system projectFilesys |                       |
        |                       | tem,                  |                       |
        |                       |           BuildTarget |                       |
        |                       |  buildTarget,         |                       |
        |                       |                    Pa |                       |
        |                       | th sdkPath,           |                       |
        |                       |                  Tool |                       |
        |                       |  lipo,                |                       |
        |                       |             Path bund |                       |
        |                       | leBinaryPath,         |                       |
        |                       |                    co |                       |
        |                       | m.facebook.buck.apple |                       |
        |                       | .AppleBundleDestinati |                       |
        |                       | ons destinations,     |                       |
        |                       |                       |                       |
        |                       |   boolean isAppClip)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `addVariantFileProc   | ::: block             |
        |                       | essingSteps​(AppleBund | Adds Variant file     |
        |                       | leResources resources | processing steps to a |
        |                       | ,                     | build rule            |
        |                       |           BuildContex | :::                   |
        |                       | t context,            |                       |
        |                       |                    Pa |                       |
        |                       | th dirRoot,           |                       |
        |                       |                     c |                       |
        |                       | om.facebook.buck.appl |                       |
        |                       | e.AppleBundleDestinat |                       |
        |                       | ions destinations,    |                       |
        |                       |                       |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist.Builder<Step> ste |                       |
        |                       | psBuilder,            |                       |
        |                       |                    Pr |                       |
        |                       | ojectFilesystem proje |                       |
        |                       | ctFilesystem,         |                       |
        |                       |                       |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList<S |                       |
        |                       | tring> ibtoolFlags,   |                       |
        |                       |                       |                       |
        |                       |        boolean isLega |                       |
        |                       | cyWatchApp,           |                       |
        |                       |                     A |                       |
        |                       | pplePlatform platform |                       |
        |                       | ,                     |                       |
        |                       |           Logger LOG, |                       |
        |                       |                       |                       |
        |                       |          Tool ibtool, |                       |
        |                       |                       |                       |
        |                       |          boolean ibto |                       |
        |                       | olModuleFlag,         |                       |
        |                       |                       |                       |
        |                       |  BuildTarget buildTar |                       |
        |                       | get,                  |                       |
        |                       |              Optional |                       |
        |                       | <String> binaryName)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#BASE_IBTOOL_FLAGS}

        -   #### BASE_IBTOOL_FLAGS

                public static final com.google.common.collect.ImmutableList<String> BASE_IBTOOL_FLAGS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addStoryboardProcessingSteps(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableList.Builder,com.google.common.collect.ImmutableList,boolean,com.facebook.buck.apple.toolchain.ApplePlatform,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.util.log.Logger,com.facebook.buck.core.toolchain.tool.Tool,boolean,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### addStoryboardProcessingSteps

            ``` methodSignature
            public static void addStoryboardProcessingSteps​(SourcePathResolverAdapter resolver,
                                                            Path sourcePath,
                                                            Path destinationPath,
                                                            com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                            com.google.common.collect.ImmutableList<String> ibtoolFlags,
                                                            boolean isLegacyWatchApp,
                                                            ApplePlatform platform,
                                                            ProjectFilesystem projectFilesystem,
                                                            Logger LOG,
                                                            Tool ibtool,
                                                            boolean ibtoolModuleFlag,
                                                            BuildTarget buildTarget,
                                                            Optional<String> binaryName)
            ```

            ::: block
            Add Storyboard processing ibtool steps to a build rule
            :::

        []{#addVariantFileProcessingSteps(com.facebook.buck.apple.AppleBundleResources,com.facebook.buck.core.build.context.BuildContext,java.nio.file.Path,com.facebook.buck.apple.AppleBundleDestinations,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,boolean,com.facebook.buck.apple.toolchain.ApplePlatform,com.facebook.buck.core.util.log.Logger,com.facebook.buck.core.toolchain.tool.Tool,boolean,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### addVariantFileProcessingSteps

            ``` methodSignature
            public static void addVariantFileProcessingSteps​(AppleBundleResources resources,
                                                             BuildContext context,
                                                             Path dirRoot,
                                                             com.facebook.buck.apple.AppleBundleDestinations destinations,
                                                             com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                             ProjectFilesystem projectFilesystem,
                                                             com.google.common.collect.ImmutableList<String> ibtoolFlags,
                                                             boolean isLegacyWatchApp,
                                                             ApplePlatform platform,
                                                             Logger LOG,
                                                             Tool ibtool,
                                                             boolean ibtoolModuleFlag,
                                                             BuildTarget buildTarget,
                                                             Optional<String> binaryName)
            ```

            ::: block
            Adds Variant file processing steps to a build rule
            :::

        []{#addFrameworksProcessingSteps(java.util.Set,java.nio.file.Path,com.facebook.buck.apple.AppleBundleDestinations,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList.Builder)}

        -   #### addFrameworksProcessingSteps

            ``` methodSignature
            public static void addFrameworksProcessingSteps​(Set<SourcePath> frameworks,
                                                            Path dirRoot,
                                                            com.facebook.buck.apple.AppleBundleDestinations destinations,
                                                            com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                            BuildContext context,
                                                            ProjectFilesystem projectFilesystem,
                                                            com.google.common.collect.ImmutableList.Builder<Path> codeSignOnCopyPathsBuilder)
            ```

            ::: block
            Adds framework processing steps to a build rule
            :::

        []{#addSwiftStdlibStepIfNeeded(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,java.nio.file.Path,java.util.Optional,com.google.common.collect.ImmutableList.Builder,boolean,java.lang.String,boolean,boolean,java.util.Optional,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path,com.facebook.buck.core.toolchain.tool.Tool,java.nio.file.Path,com.facebook.buck.apple.AppleBundleDestinations,boolean)}

        -   #### addSwiftStdlibStepIfNeeded

            ``` methodSignature
            public static void addSwiftStdlibStepIfNeeded​(SourcePathResolverAdapter resolver,
                                                          Path destinationPath,
                                                          Path bundleRoot,
                                                          Optional<java.util.function.Supplier<CodeSignIdentity>> codeSignIdentitySupplier,
                                                          com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                          boolean isForPackaging,
                                                          String bundleExtension,
                                                          boolean copySwiftStdlibToFrameworks,
                                                          boolean useLipoThin,
                                                          Optional<Tool> swiftStdlibTool,
                                                          ProjectFilesystem projectFilesystem,
                                                          BuildTarget buildTarget,
                                                          Path sdkPath,
                                                          Tool lipo,
                                                          Path bundleBinaryPath,
                                                          com.facebook.buck.apple.AppleBundleDestinations destinations,
                                                          boolean isAppClip)
            ```

            ::: block
            Adds the swift stdlib to the bundle if needed
            :::

        []{#addResourceProcessingSteps(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableList.Builder,com.google.common.collect.ImmutableList,com.facebook.buck.io.filesystem.ProjectFilesystem,boolean,com.facebook.buck.apple.toolchain.ApplePlatform,com.facebook.buck.core.util.log.Logger,com.facebook.buck.core.toolchain.tool.Tool,boolean,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### addResourceProcessingSteps

            ``` methodSignature
            public static void addResourceProcessingSteps​(SourcePathResolverAdapter resolver,
                                                          Path sourcePath,
                                                          Path destinationPath,
                                                          com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                          com.google.common.collect.ImmutableList<String> ibtoolFlags,
                                                          ProjectFilesystem projectFilesystem,
                                                          boolean isLegacyWatchApp,
                                                          ApplePlatform platform,
                                                          Logger LOG,
                                                          Tool ibtool,
                                                          boolean ibtoolModuleFlag,
                                                          BuildTarget buildTarget,
                                                          Optional<String> binaryName)
            ```

            ::: block
            Adds Resources processing steps to a build rule
            :::

        []{#addStepsToCopyResources(com.facebook.buck.core.build.context.BuildContext,com.google.common.collect.ImmutableList.Builder,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.apple.AppleBundleResources,boolean,java.nio.file.Path,com.facebook.buck.apple.AppleBundleDestinations,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,boolean,com.facebook.buck.apple.toolchain.ApplePlatform,com.facebook.buck.core.util.log.Logger,com.facebook.buck.core.toolchain.tool.Tool,boolean,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### addStepsToCopyResources

            ``` methodSignature
            public static void addStepsToCopyResources​(BuildContext context,
                                                       com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder,
                                                       com.google.common.collect.ImmutableList.Builder<Path> codeSignOnCopyPathsBuilder,
                                                       AppleBundleResources resources,
                                                       boolean verifyResources,
                                                       Path dirRoot,
                                                       com.facebook.buck.apple.AppleBundleDestinations destinations,
                                                       ProjectFilesystem projectFilesystem,
                                                       com.google.common.collect.ImmutableList<String> ibtoolFlags,
                                                       boolean isLegacyWatchApp,
                                                       ApplePlatform platform,
                                                       Logger LOG,
                                                       Tool ibtool,
                                                       boolean ibtoolModuleFlag,
                                                       BuildTarget buildTarget,
                                                       Optional<String> binaryName)
            ```

            ::: block
            Adds required copy resources steps
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
