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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class XcodeNativeTargetGenerator {#class-xcodenativetargetgenerator .title title="Class XcodeNativeTargetGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.XcodeNativeTargetGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class XcodeNativeTargetGenerator
        extends Object

    ::: block
    Generates all the target attributes `GeneratedTargetAttributes` to
    be written into a
    [`PBXNativeTarget`](../../../apple/xcode/xcodeproj/PBXNativeTarget.html "class in com.facebook.buck.apple.xcode.xcodeproj").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `XcodeNativeTa        | ::: block             |
        |                       | rgetGenerator.Result` | The result of         |
        |                       |                       | materializing the     |
        |                       |                       | build target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `XcodeNativeTargetGenerator​(XCodeDescriptions xcodeDescriptions,                           TargetGraph targetGraph,                           AppleDependenciesCache dependenciesCache,                           ProjectGenerationStateCache projGenerationStateCache,                           ProjectFilesystem projectFilesystem,                           Path sourceRoot,                           String buildFileName,                           com.facebook.buck.features.apple.projectV2.PathRelativizer pathRelativizer,                           SourcePathResolverAdapter defaultPathResolver,                           ProjectSourcePathResolver projectSourcePathResolver,                           ProjectGeneratorOptions options,                           CxxPlatform defaultCxxPlatform,                           com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,                           java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode,                           HalideBuckConfig halideBuckConfig,                           com.facebook.buck.features.apple.projectV2.HeaderSearchPaths headerSearchPaths,                           CxxBuckConfig cxxBuckConfig,                           AppleConfig appleConfig,                           SwiftBuckConfig swiftBuckConfig,                           SwiftAttributeParser swiftAttributeParser,                           com.facebook.buck.features.apple.projectV2.FlagParser flagParser,                           Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle,                           AbstractPBXObjectFactory objectFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com           | `computeS             | ::: block             |
        | .google.common.collec | haredLibrariesToBundl | Generate a mapping    |
        | t.ImmutableMap<BuildT | es​(com.google.common. | from libraries to the |
        | arget,​TargetNode<?>>` | collect.ImmutableSet< | framework bundles     |
        |                       | TargetNode<?>> target | that include them.    |
        |                       | Nodes,                | :::                   |
        |                       |                  Targ |                       |
        |                       | etGraph targetGraph)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeNativeTa        | `generateTarget​(Targe | ::: block             |
        | rgetGenerator.Result` | tNode<?> targetNode)` | Generates the target  |
        |                       |                       | node.                 |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.apple.AppleDependenciesCache,com.facebook.buck.features.apple.projectV2.ProjectGenerationStateCache,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.lang.String,com.facebook.buck.features.apple.projectV2.PathRelativizer,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.features.apple.projectV2.ProjectSourcePathResolver,com.facebook.buck.features.apple.projectV2.ProjectGeneratorOptions,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSet,java.util.function.Function,com.facebook.buck.features.halide.HalideBuckConfig,com.facebook.buck.features.apple.projectV2.HeaderSearchPaths,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.apple.AppleConfig,com.facebook.buck.swift.SwiftBuckConfig,com.facebook.buck.features.apple.projectV2.SwiftAttributeParser,com.facebook.buck.features.apple.projectV2.FlagParser,java.util.Optional,com.facebook.buck.apple.xcode.AbstractPBXObjectFactory)}

        -   #### XcodeNativeTargetGenerator

                public XcodeNativeTargetGenerator​(XCodeDescriptions xcodeDescriptions,
                                                  TargetGraph targetGraph,
                                                  AppleDependenciesCache dependenciesCache,
                                                  ProjectGenerationStateCache projGenerationStateCache,
                                                  ProjectFilesystem projectFilesystem,
                                                  Path sourceRoot,
                                                  String buildFileName,
                                                  com.facebook.buck.features.apple.projectV2.PathRelativizer pathRelativizer,
                                                  SourcePathResolverAdapter defaultPathResolver,
                                                  ProjectSourcePathResolver projectSourcePathResolver,
                                                  ProjectGeneratorOptions options,
                                                  CxxPlatform defaultCxxPlatform,
                                                  com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,
                                                  java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode,
                                                  HalideBuckConfig halideBuckConfig,
                                                  com.facebook.buck.features.apple.projectV2.HeaderSearchPaths headerSearchPaths,
                                                  CxxBuckConfig cxxBuckConfig,
                                                  AppleConfig appleConfig,
                                                  SwiftBuckConfig swiftBuckConfig,
                                                  SwiftAttributeParser swiftAttributeParser,
                                                  com.facebook.buck.features.apple.projectV2.FlagParser flagParser,
                                                  Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle,
                                                  AbstractPBXObjectFactory objectFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#generateTarget(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### generateTarget

            ``` methodSignature
            public XcodeNativeTargetGenerator.Result generateTarget​(TargetNode<?> targetNode)
                                                             throws IOException
            ```

            ::: block
            Generates the target node.
            :::

            [Parameters:]{.paramLabel}
            :   `targetNode` - The node to generate

            [Returns:]{.returnLabel}
            :   A result with all of the data aggregated for this node.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#computeSharedLibrariesToBundles(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### computeSharedLibrariesToBundles

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>> computeSharedLibrariesToBundles​(com.google.common.collect.ImmutableSet<TargetNode<?>> targetNodes,
                                                                                                                                  TargetGraph targetGraph)
                                                                                                                           throws HumanReadableException
            ```

            ::: block
            Generate a mapping from libraries to the framework bundles
            that include them.
            :::

            [Throws:]{.throwsLabel}
            :   `HumanReadableException`
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
