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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleLibraryDescriptionSwiftEnhancer {#class-applelibrarydescriptionswiftenhancer .title title="Class AppleLibraryDescriptionSwiftEnhancer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleLibraryDescriptionSwiftEnhancer

::: description
-   

    ------------------------------------------------------------------------

        public class AppleLibraryDescriptionSwiftEnhancer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `AppleLibraryDescriptionSwiftEnhancer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static BuildTarget`  | `createBuildTargetFor |                       |
        |                       | ObjCGeneratedHeaderBu |                       |
        |                       | ildRule​(BuildTarget b |                       |
        |                       | uildTarget,           |                       |
        |                       |                       |                       |
        |                       |                   Hea |                       |
        |                       | derVisibility headerV |                       |
        |                       | isibility,            |                       |
        |                       |                       |                       |
        |                       |                  CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `creat                |                       |
        |                       | eBuildTargetForSwiftC |                       |
        |                       | ompile​(BuildTarget ta |                       |
        |                       | rget,                 |                       |
        |                       |                  CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildRule`    | `createObjCG          |                       |
        |                       | eneratedHeaderBuildRu |                       |
        |                       | le​(BuildTarget buildT |                       |
        |                       | arget,                |                       |
        |                       |                     P |                       |
        |                       | rojectFilesystem proj |                       |
        |                       | ectFilesystem,        |                       |
        |                       |                       |                       |
        |                       |        ActionGraphBui |                       |
        |                       | lder graphBuilder,    |                       |
        |                       |                       |                       |
        |                       |            CxxPlatfor |                       |
        |                       | m cxxPlatform,        |                       |
        |                       |                       |                       |
        |                       |        HeaderVisibili |                       |
        |                       | ty headerVisibility)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildRule`    | `                     |                       |
        |                       | createSwiftCompileRul |                       |
        |                       | e​(BuildTarget target, |                       |
        |                       |                       |                       |
        |                       |   CellPathResolver ce |                       |
        |                       | llRoots,              |                       |
        |                       |           ActionGraph |                       |
        |                       | Builder graphBuilder, |                       |
        |                       |                       |                       |
        |                       |   AppleNativeTargetDe |                       |
        |                       | scriptionArg args,    |                       |
        |                       |                     P |                       |
        |                       | rojectFilesystem file |                       |
        |                       | system,               |                       |
        |                       |          CxxPlatform  |                       |
        |                       | platform,             |                       |
        |                       |            AppleCxxPl |                       |
        |                       | atform applePlatform, |                       |
        |                       |                       |                       |
        |                       |   SwiftBuckConfig swi |                       |
        |                       | ftBuckConfig,         |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSet<CxxPrepro |                       |
        |                       | cessorInput> inputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getObjCGeneratedHe   |                       |
        | static com.google.com | ader​(BuildTarget buil |                       |
        | mon.collect.Immutable | dTarget,              |                       |
        | Map<Path,​SourcePath>` |           ActionGraph |                       |
        |                       | Builder graphBuilder, |                       |
        |                       |                       |                       |
        |                       |   CxxPlatform cxxPlat |                       |
        |                       | form,                 |                       |
        |                       |        HeaderVisibili |                       |
        |                       | ty headerVisibility)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `getPr                | ::: block             |
        | c com.google.common.c | eprocessorInputsForAp | Returns transitive    |
        | ollect.ImmutableSet<C | pleLibrary​(BuildTarge | preprocessor inputs   |
        | xxPreprocessorInput>` | t target,             | excluding those from  |
        |                       |                       | the swift delegate of |
        |                       |     ActionGraphBuilde | the given CxxLibrary. |
        |                       | r graphBuilder,       | :::                   |
        |                       |                       |                       |
        |                       |           CxxPlatform |                       |
        |                       |  platform,            |                       |
        |                       |                       |                       |
        |                       |      AppleNativeTarge |                       |
        |                       | tDescriptionArg arg)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AppleLibraryDescriptionSwiftEnhancer

                public AppleLibraryDescriptionSwiftEnhancer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createSwiftCompileRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.apple.AppleNativeTargetDescriptionArg,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.apple.toolchain.AppleCxxPlatform,com.facebook.buck.swift.SwiftBuckConfig,com.google.common.collect.ImmutableSet)}

        -   #### createSwiftCompileRule

            ``` methodSignature
            public static BuildRule createSwiftCompileRule​(BuildTarget target,
                                                           CellPathResolver cellRoots,
                                                           ActionGraphBuilder graphBuilder,
                                                           AppleNativeTargetDescriptionArg args,
                                                           ProjectFilesystem filesystem,
                                                           CxxPlatform platform,
                                                           AppleCxxPlatform applePlatform,
                                                           SwiftBuckConfig swiftBuckConfig,
                                                           com.google.common.collect.ImmutableSet<CxxPreprocessorInput> inputs)
            ```

        []{#getPreprocessorInputsForAppleLibrary(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.apple.AppleNativeTargetDescriptionArg)}

        -   #### getPreprocessorInputsForAppleLibrary

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<CxxPreprocessorInput> getPreprocessorInputsForAppleLibrary​(BuildTarget target,
                                                                                                                            ActionGraphBuilder graphBuilder,
                                                                                                                            CxxPlatform platform,
                                                                                                                            AppleNativeTargetDescriptionArg arg)
            ```

            ::: block
            Returns transitive preprocessor inputs excluding those from
            the swift delegate of the given CxxLibrary.
            :::

        []{#createObjCGeneratedHeaderBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.HeaderVisibility)}

        -   #### createObjCGeneratedHeaderBuildRule

            ``` methodSignature
            public static BuildRule createObjCGeneratedHeaderBuildRule​(BuildTarget buildTarget,
                                                                       ProjectFilesystem projectFilesystem,
                                                                       ActionGraphBuilder graphBuilder,
                                                                       CxxPlatform cxxPlatform,
                                                                       HeaderVisibility headerVisibility)
            ```

        []{#getObjCGeneratedHeader(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.HeaderVisibility)}

        -   #### getObjCGeneratedHeader

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> getObjCGeneratedHeader​(BuildTarget buildTarget,
                                                                                                               ActionGraphBuilder graphBuilder,
                                                                                                               CxxPlatform cxxPlatform,
                                                                                                               HeaderVisibility headerVisibility)
            ```

        []{#createBuildTargetForObjCGeneratedHeaderBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.HeaderVisibility,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### createBuildTargetForObjCGeneratedHeaderBuildRule

            ``` methodSignature
            public static BuildTarget createBuildTargetForObjCGeneratedHeaderBuildRule​(BuildTarget buildTarget,
                                                                                       HeaderVisibility headerVisibility,
                                                                                       CxxPlatform cxxPlatform)
            ```

        []{#createBuildTargetForSwiftCompile(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### createBuildTargetForSwiftCompile

            ``` methodSignature
            public static BuildTarget createBuildTargetForSwiftCompile​(BuildTarget target,
                                                                       CxxPlatform cxxPlatform)
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
