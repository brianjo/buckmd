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

## Class AppleDescriptions {#class-appledescriptions .title title="Class AppleDescriptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleDescriptions

::: description
-   

    ------------------------------------------------------------------------

        public class AppleDescriptions
        extends Object

    ::: block
    Common logic for a
    [`DescriptionWithTargetGraph`](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")
    that creates Apple target rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                Field                                                        Description
          -------------------------------- ------------------------------------------------------------ -------------
          `static Flavor`                  `FRAMEWORK_FLAVOR`                                            
          `static FlavorDomain<Boolean>`   `INCLUDE_FRAMEWORKS`                                          
          `static Flavor`                  `INCLUDE_FRAMEWORKS_FLAVOR`                                   
          `static Flavor`                  `NO_INCLUDE_FRAMEWORKS_FLAVOR`                                
          `static Flavor`                  `SWIFT_COMPILE_FLAVOR`                                        
          `static Flavor`                  `SWIFT_EXPORTED_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR`    
          `static Flavor`                  `SWIFT_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR`             
          `static Flavor`                  `SWIFT_UNDERLYING_MODULE_FLAVOR`                              

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static c             | `con                  |                       |
        | om.google.common.coll | vertAppleHeadersToPri |                       |
        | ect.ImmutableSortedMa | vateCxxHeaders​(BuildT |                       |
        | p<String,​SourcePath>` | arget buildTarget,    |                       |
        |                       |                       |                       |
        |                       |                java.u |                       |
        |                       | til.function.Function |                       |
        |                       | <SourcePath,​Path> pat |                       |
        |                       | hResolver,            |                       |
        |                       |                       |                       |
        |                       |        Path headerPat |                       |
        |                       | hPrefix,              |                       |
        |                       |                       |                       |
        |                       |      CxxLibraryDescri |                       |
        |                       | ption.CommonArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static c             | `convertAppleHeadersT |                       |
        | om.google.common.coll | oPublicCxxHeaders​(Bui |                       |
        | ect.ImmutableSortedMa | ldTarget buildTarget, |                       |
        | p<String,​SourcePath>` |                       |                       |
        |                       |                  java |                       |
        |                       | .util.function.Functi |                       |
        |                       | on<SourcePath,​Path> p |                       |
        |                       | athResolver,          |                       |
        |                       |                       |                       |
        |                       |         Path headerPa |                       |
        |                       | thPrefix,             |                       |
        |                       |                       |                       |
        |                       |      CxxLibraryDescri |                       |
        |                       | ption.CommonArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static c             | `conv                 |                       |
        | om.google.common.coll | ertHeadersToPrivateCx |                       |
        | ect.ImmutableSortedMa | xHeaders​(BuildTarget  |                       |
        | p<String,​SourcePath>` | buildTarget,          |                       |
        |                       |                       |                       |
        |                       |     java.util.functio |                       |
        |                       | n.Function<SourcePath |                       |
        |                       | ,​Path> pathResolver,  |                       |
        |                       |                       |                       |
        |                       |             Path head |                       |
        |                       | erPathPrefix,         |                       |
        |                       |                       |                       |
        |                       |      SourceSortedSet  |                       |
        |                       | privateSourceSet,     |                       |
        |                       |                       |                       |
        |                       |          SourceSorted |                       |
        |                       | Set publicSourceSet)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static c             | `convertHead          |                       |
        | om.google.common.coll | ersToPublicCxxHeaders |                       |
        | ect.ImmutableSortedMa | ​(BuildTarget buildTar |                       |
        | p<String,​SourcePath>` | get,                  |                       |
        |                       |                 java. |                       |
        |                       | util.function.Functio |                       |
        |                       | n<SourcePath,​Path> pa |                       |
        |                       | thResolver,           |                       |
        |                       |                       |                       |
        |                       |   Path headerPathPref |                       |
        |                       | ix,                   |                       |
        |                       |                Source |                       |
        |                       | SortedSet sourceSet)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Optiona       | `createBuild          |                       |
        | l<AppleAssetCatalog>` | RuleForTransitiveAsse |                       |
        |                       | tCatalogDependencies​( |                       |
        |                       | XCodeDescriptions xco |                       |
        |                       | deDescriptions,       |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |      TargetGraph targ |                       |
        |                       | etGraph,              |                       |
        |                       |                       |                       |
        |                       |                    Bu |                       |
        |                       | ildTarget buildTarget |                       |
        |                       | ,                     |                       |
        |                       |                       |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem projectFiles |                       |
        |                       | ystem,                |                       |
        |                       |                       |                       |
        |                       |                  Sour |                       |
        |                       | cePathRuleFinder rule |                       |
        |                       | Finder,               |                       |
        |                       |                       |                       |
        |                       |                   Opt |                       |
        |                       | ional<String> product |                       |
        |                       | Type,                 |                       |
        |                       |                       |                       |
        |                       |                 Apple |                       |
        |                       | Platform applePlatfor |                       |
        |                       | m,                    |                       |
        |                       |                       |                       |
        |                       |              String t |                       |
        |                       | argetSDKVersion,      |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |       Tool actool,    |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |         AppleAssetCat |                       |
        |                       | alog.ValidationType a |                       |
        |                       | ssetCatalogValidation |                       |
        |                       | ,                     |                       |
        |                       |                       |                       |
        |                       |             AppleAsse |                       |
        |                       | tCatalogsCompilationO |                       |
        |                       | ptions appleAssetCata |                       |
        |                       | logsCompilationOption |                       |
        |                       | s,                    |                       |
        |                       |                       |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Opt           | `createBuildRulesFor  |                       |
        | ional<CoreDataModel>` | CoreDataDependencies​( |                       |
        |                       | XCodeDescriptions xco |                       |
        |                       | deDescriptions,       |                       |
        |                       |                       |                       |
        |                       |              TargetGr |                       |
        |                       | aph targetGraph,      |                       |
        |                       |                       |                       |
        |                       |               BuildTa |                       |
        |                       | rget buildTarget,     |                       |
        |                       |                       |                       |
        |                       |                Projec |                       |
        |                       | tFilesystem projectFi |                       |
        |                       | lesystem,             |                       |
        |                       |                       |                       |
        |                       |        BuildRuleParam |                       |
        |                       | s params,             |                       |
        |                       |                       |                       |
        |                       |        String moduleN |                       |
        |                       | ame,                  |                       |
        |                       |                       |                       |
        |                       |   AppleCxxPlatform ap |                       |
        |                       | pleCxxPlatform,       |                       |
        |                       |                       |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Opti          | `cre                  |                       |
        | onal<SceneKitAssets>` | ateBuildRulesForScene |                       |
        |                       | KitAssetsDependencies |                       |
        |                       | ​(XCodeDescriptions xc |                       |
        |                       | odeDescriptions,      |                       |
        |                       |                       |                       |
        |                       |                     T |                       |
        |                       | argetGraph targetGrap |                       |
        |                       | h,                    |                       |
        |                       |                       |                       |
        |                       |       BuildTarget bui |                       |
        |                       | ldTarget,             |                       |
        |                       |                       |                       |
        |                       |              ProjectF |                       |
        |                       | ilesystem projectFile |                       |
        |                       | system,               |                       |
        |                       |                       |                       |
        |                       |            BuildRuleP |                       |
        |                       | arams params,         |                       |
        |                       |                       |                       |
        |                       |                  Appl |                       |
        |                       | eCxxPlatform appleCxx |                       |
        |                       | Platform,             |                       |
        |                       |                       |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `flavorsDoNotAl       |                       |
        |                       | lowLinkerMapMode​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getHeaderPathPref    |                       |
        |                       | ix​(AppleNativeTargetD |                       |
        |                       | escriptionArg arg,    |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `g                    | ::: block             |
        |                       | etTargetPlatformBinar | Returns a build       |
        |                       | y​(Optional<BuildTarge | target of the apple   |
        |                       | t> binary,            | binary for the        |
        |                       |              Optional | requested target      |
        |                       | <PatternMatchedCollec | platform.             |
        |                       | tion<BuildTarget>> pl | :::                   |
        |                       | atformBinary,         |                       |
        |                       |                 Flavo |                       |
        |                       | r cxxPlatformFlavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `populateCx           |                       |
        |                       | xBinaryDescriptionArg |                       |
        |                       | ​(ActionGraphBuilder g |                       |
        |                       | raphBuilder,          |                       |
        |                       |                       |                       |
        |                       |   CxxBinaryDescriptio |                       |
        |                       | nArg.Builder output,  |                       |
        |                       |                       |                       |
        |                       |           Optional<Un |                       |
        |                       | resolvedAppleCxxPlatf |                       |
        |                       | orm> appleCxxPlatform |                       |
        |                       | ,                     |                       |
        |                       |             AppleNati |                       |
        |                       | veTargetDescriptionAr |                       |
        |                       | g arg,                |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `populateCxxLibr      |                       |
        |                       | aryDescriptionArg​(Bui |                       |
        |                       | ldRuleResolver ruleRe |                       |
        |                       | solver,               |                       |
        |                       |                    Cx |                       |
        |                       | xLibraryDescriptionAr |                       |
        |                       | g.Builder output,     |                       |
        |                       |                       |                       |
        |                       |         Optional<Unre |                       |
        |                       | solvedAppleCxxPlatfor |                       |
        |                       | m> appleCxxPlatform,  |                       |
        |                       |                       |                       |
        |                       |            AppleNativ |                       |
        |                       | eTargetDescriptionArg |                       |
        |                       |  arg,                 |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `targetNode           |                       |
        |                       | ContainsSwiftSourceCo |                       |
        |                       | de​(TargetNode<? exten |                       |
        |                       | ds CxxLibraryDescript |                       |
        |                       | ion.CommonArg> node)` |                       |
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

        []{#FRAMEWORK_FLAVOR}

        -   #### FRAMEWORK_FLAVOR

                public static final Flavor FRAMEWORK_FLAVOR

        []{#SWIFT_COMPILE_FLAVOR}

        -   #### SWIFT_COMPILE_FLAVOR

                public static final Flavor SWIFT_COMPILE_FLAVOR

        []{#SWIFT_EXPORTED_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR}

        -   #### SWIFT_EXPORTED_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR

                public static final Flavor SWIFT_EXPORTED_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR

        []{#SWIFT_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR}

        -   #### SWIFT_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR

                public static final Flavor SWIFT_OBJC_GENERATED_HEADER_SYMLINK_TREE_FLAVOR

        []{#SWIFT_UNDERLYING_MODULE_FLAVOR}

        -   #### SWIFT_UNDERLYING_MODULE_FLAVOR

                public static final Flavor SWIFT_UNDERLYING_MODULE_FLAVOR

        []{#INCLUDE_FRAMEWORKS_FLAVOR}

        -   #### INCLUDE_FRAMEWORKS_FLAVOR

                public static final Flavor INCLUDE_FRAMEWORKS_FLAVOR

        []{#NO_INCLUDE_FRAMEWORKS_FLAVOR}

        -   #### NO_INCLUDE_FRAMEWORKS_FLAVOR

                public static final Flavor NO_INCLUDE_FRAMEWORKS_FLAVOR

        []{#INCLUDE_FRAMEWORKS}

        -   #### INCLUDE_FRAMEWORKS

                public static final FlavorDomain<Boolean> INCLUDE_FRAMEWORKS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHeaderPathPrefix(com.facebook.buck.apple.AppleNativeTargetDescriptionArg,com.facebook.buck.core.model.BuildTarget)}

        -   #### getHeaderPathPrefix

            ``` methodSignature
            public static Path getHeaderPathPrefix​(AppleNativeTargetDescriptionArg arg,
                                                   BuildTarget buildTarget)
            ```

        []{#convertAppleHeadersToPublicCxxHeaders(com.facebook.buck.core.model.BuildTarget,java.util.function.Function,java.nio.file.Path,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### convertAppleHeadersToPublicCxxHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<String,​SourcePath> convertAppleHeadersToPublicCxxHeaders​(BuildTarget buildTarget,
                                                                                                                                      java.util.function.Function<SourcePath,​Path> pathResolver,
                                                                                                                                      Path headerPathPrefix,
                                                                                                                                      CxxLibraryDescription.CommonArg arg)
            ```

        []{#convertHeadersToPublicCxxHeaders(com.facebook.buck.core.model.BuildTarget,java.util.function.Function,java.nio.file.Path,com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### convertHeadersToPublicCxxHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<String,​SourcePath> convertHeadersToPublicCxxHeaders​(BuildTarget buildTarget,
                                                                                                                                 java.util.function.Function<SourcePath,​Path> pathResolver,
                                                                                                                                 Path headerPathPrefix,
                                                                                                                                 SourceSortedSet sourceSet)
            ```

        []{#convertAppleHeadersToPrivateCxxHeaders(com.facebook.buck.core.model.BuildTarget,java.util.function.Function,java.nio.file.Path,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### convertAppleHeadersToPrivateCxxHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<String,​SourcePath> convertAppleHeadersToPrivateCxxHeaders​(BuildTarget buildTarget,
                                                                                                                                       java.util.function.Function<SourcePath,​Path> pathResolver,
                                                                                                                                       Path headerPathPrefix,
                                                                                                                                       CxxLibraryDescription.CommonArg arg)
            ```

        []{#convertHeadersToPrivateCxxHeaders(com.facebook.buck.core.model.BuildTarget,java.util.function.Function,java.nio.file.Path,com.facebook.buck.rules.coercer.SourceSortedSet,com.facebook.buck.rules.coercer.SourceSortedSet)}

        -   #### convertHeadersToPrivateCxxHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<String,​SourcePath> convertHeadersToPrivateCxxHeaders​(BuildTarget buildTarget,
                                                                                                                                  java.util.function.Function<SourcePath,​Path> pathResolver,
                                                                                                                                  Path headerPathPrefix,
                                                                                                                                  SourceSortedSet privateSourceSet,
                                                                                                                                  SourceSortedSet publicSourceSet)
            ```

        []{#populateCxxBinaryDescriptionArg(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.CxxBinaryDescriptionArg.Builder,java.util.Optional,com.facebook.buck.apple.AppleNativeTargetDescriptionArg,com.facebook.buck.core.model.BuildTarget)}

        -   #### populateCxxBinaryDescriptionArg

            ``` methodSignature
            public static void populateCxxBinaryDescriptionArg​(ActionGraphBuilder graphBuilder,
                                                               CxxBinaryDescriptionArg.Builder output,
                                                               Optional<UnresolvedAppleCxxPlatform> appleCxxPlatform,
                                                               AppleNativeTargetDescriptionArg arg,
                                                               BuildTarget buildTarget)
            ```

        []{#populateCxxLibraryDescriptionArg(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.cxx.CxxLibraryDescriptionArg.Builder,java.util.Optional,com.facebook.buck.apple.AppleNativeTargetDescriptionArg,com.facebook.buck.core.model.BuildTarget)}

        -   #### populateCxxLibraryDescriptionArg

            ``` methodSignature
            public static void populateCxxLibraryDescriptionArg​(BuildRuleResolver ruleResolver,
                                                                CxxLibraryDescriptionArg.Builder output,
                                                                Optional<UnresolvedAppleCxxPlatform> appleCxxPlatform,
                                                                AppleNativeTargetDescriptionArg arg,
                                                                BuildTarget buildTarget)
            ```

        []{#createBuildRuleForTransitiveAssetCatalogDependencies(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional,com.facebook.buck.apple.toolchain.ApplePlatform,java.lang.String,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.apple.AppleAssetCatalog.ValidationType,com.facebook.buck.apple.AppleAssetCatalogsCompilationOptions,java.util.function.Predicate)}

        -   #### createBuildRuleForTransitiveAssetCatalogDependencies

            ``` methodSignature
            public static Optional<AppleAssetCatalog> createBuildRuleForTransitiveAssetCatalogDependencies​(XCodeDescriptions xcodeDescriptions,
                                                                                                           TargetGraph targetGraph,
                                                                                                           BuildTarget buildTarget,
                                                                                                           ProjectFilesystem projectFilesystem,
                                                                                                           SourcePathRuleFinder ruleFinder,
                                                                                                           Optional<String> productType,
                                                                                                           ApplePlatform applePlatform,
                                                                                                           String targetSDKVersion,
                                                                                                           Tool actool,
                                                                                                           AppleAssetCatalog.ValidationType assetCatalogValidation,
                                                                                                           AppleAssetCatalogsCompilationOptions appleAssetCatalogsCompilationOptions,
                                                                                                           java.util.function.Predicate<BuildTarget> filter)
            ```

        []{#createBuildRulesForCoreDataDependencies(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,java.lang.String,com.facebook.buck.apple.toolchain.AppleCxxPlatform,java.util.function.Predicate)}

        -   #### createBuildRulesForCoreDataDependencies

            ``` methodSignature
            public static Optional<CoreDataModel> createBuildRulesForCoreDataDependencies​(XCodeDescriptions xcodeDescriptions,
                                                                                          TargetGraph targetGraph,
                                                                                          BuildTarget buildTarget,
                                                                                          ProjectFilesystem projectFilesystem,
                                                                                          BuildRuleParams params,
                                                                                          String moduleName,
                                                                                          AppleCxxPlatform appleCxxPlatform,
                                                                                          java.util.function.Predicate<BuildTarget> filter)
            ```

        []{#createBuildRulesForSceneKitAssetsDependencies(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.apple.toolchain.AppleCxxPlatform,java.util.function.Predicate)}

        -   #### createBuildRulesForSceneKitAssetsDependencies

            ``` methodSignature
            public static Optional<SceneKitAssets> createBuildRulesForSceneKitAssetsDependencies​(XCodeDescriptions xcodeDescriptions,
                                                                                                 TargetGraph targetGraph,
                                                                                                 BuildTarget buildTarget,
                                                                                                 ProjectFilesystem projectFilesystem,
                                                                                                 BuildRuleParams params,
                                                                                                 AppleCxxPlatform appleCxxPlatform,
                                                                                                 java.util.function.Predicate<BuildTarget> filter)
            ```

        []{#getTargetPlatformBinary(java.util.Optional,java.util.Optional,com.facebook.buck.core.model.Flavor)}

        -   #### getTargetPlatformBinary

            ``` methodSignature
            public static BuildTarget getTargetPlatformBinary​(Optional<BuildTarget> binary,
                                                              Optional<PatternMatchedCollection<BuildTarget>> platformBinary,
                                                              Flavor cxxPlatformFlavor)
            ```

            ::: block
            Returns a build target of the apple binary for the requested
            target platform.
            By default it\'s the binary that was provided using `binary`
            attribute, but in case `platform_binary` is specified and
            one of its patterns matches the target platform, it will be
            returned instead.
            :::

        []{#flavorsDoNotAllowLinkerMapMode(com.facebook.buck.core.model.BuildTarget)}

        -   #### flavorsDoNotAllowLinkerMapMode

            ``` methodSignature
            public static boolean flavorsDoNotAllowLinkerMapMode​(BuildTarget buildTarget)
            ```

        []{#targetNodeContainsSwiftSourceCode(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### targetNodeContainsSwiftSourceCode

            ``` methodSignature
            public static boolean targetNodeContainsSwiftSourceCode​(TargetNode<? extends CxxLibraryDescription.CommonArg> node)
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
