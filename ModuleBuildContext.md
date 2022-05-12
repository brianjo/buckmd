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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class ModuleBuildContext {#class-modulebuildcontext .title title="Class ModuleBuildContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.ModuleBuildContext

::: description
-   

    ------------------------------------------------------------------------

        public class ModuleBuildContext
        extends Object

    ::: block
    Holds all of the mutable state required during
    [`IjModule`](model/IjModule.html "class in com.facebook.buck.features.project.intellij.model")
    creation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------- -------------
          `ModuleBuildContext​(com.google.common.collect.ImmutableSet<BuildTarget> circularDependencyInducingTargets)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `add                  |                       |
        |                       | CompileShadowDep​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | addDeps​(com.google.co | Record a dependency   |
        |                       | mmon.collect.Immutabl | on a                  |
        |                       | eSet<Path> sourcePath | [`BuildTar            |
        |                       | s,        Iterable<Bu | get`](../../../core/m |
        |                       | ildTarget> buildTarge | odel/BuildTarget.html |
        |                       | ts,        Dependency |  "class in com.facebo |
        |                       | Type dependencyType)` | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addDeps​(Iterable<Bu  |                       |
        |                       | ildTarget> buildTarge |                       |
        |                       | ts,        Dependency |                       |
        |                       | Type dependencyType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `add                  |                       |
        |                       | ExtraLibraryDependenc |                       |
        |                       | y​(IjLibrary library)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addExtraModuleD      |                       |
        |                       | ependency​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `add                  | ::: block             |
        |                       | GeneratedSourceCodeFo | Add BuildTarget and   |
        |                       | lder​(BuildTarget buil | its associated        |
        |                       | dTarget,              | IjFolder              |
        |                       |                 IjFol | :::                   |
        |                       | der generatedFolder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addNonS              |                       |
        |                       | ourceBuildTarget​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addSourceFol         | ::: block             |
        |                       | der​(IjFolder folder)` | Adds a source folder  |
        |                       |                       | to the context.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ensureA              |                       |
        |                       | ndroidFacetBuilder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<I           | `getAndroidFacet()`   |                       |
        | jModuleAndroidFacet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `get                  |                       |
        |                       | CompilerOutputPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getDependencies()`   |                       |
        | google.common.collect |                       |                       |
        | .ImmutableMap<BuildTa |                       |                       |
        | rget,​DependencyType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getExtraL            |                       |
        | le.common.collect.Imm | ibraryDependencies()` |                       |
        | utableSet<IjLibrary>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getExtra             |                       |
        | .google.common.collec | ModuleDependencies()` |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getGenerate          |                       |
        | mon.collect.Immutable | dSourceCodeFolders()` |                       |
        | Collection<IjFolder>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `ge                   |                       |
        |                       | tJavaLanguageLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `g                    |                       |
        |                       | etMetaInfDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `IjModuleType`        | `getModuleType()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getNon               |                       |
        | .common.collect.Immut | SourceBuildTargets()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `IjModule             | `getOrCreateA         |                       |
        | AndroidFacet.Builder` | ndroidFacetBuilder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getSourceFolders()`  |                       |
        | mon.collect.Immutable |                       |                       |
        | Collection<IjFolder>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Map<BuildTa          | `getTargetsToG        |                       |
        | rget,​List<IjFolder>>` | eneratedSourcesMap()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAndroidF           |                       |
        |                       | acetBuilderPresent()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setCompilerOutp      |                       |
        |                       | utPath​(Optional<Path> |                       |
        |                       |  compilerOutputPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setJavaLanguage      |                       |
        |                       | Level​(Optional<String |                       |
        |                       | > javaLanguageLevel)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `s                    |                       |
        |                       | etMetaInfDirectory​(Pa |                       |
        |                       | th metaInfDirectory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setModuleType​(IjMo   |                       |
        |                       | duleType moduleType)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.google.common.collect.ImmutableSet)}

        -   #### ModuleBuildContext

                public ModuleBuildContext​(com.google.common.collect.ImmutableSet<BuildTarget> circularDependencyInducingTargets)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ensureAndroidFacetBuilder()}

        -   #### ensureAndroidFacetBuilder

            ``` methodSignature
            public void ensureAndroidFacetBuilder()
            ```

        []{#getOrCreateAndroidFacetBuilder()}

        -   #### getOrCreateAndroidFacetBuilder

            ``` methodSignature
            public IjModuleAndroidFacet.Builder getOrCreateAndroidFacetBuilder()
            ```

        []{#isAndroidFacetBuilderPresent()}

        -   #### isAndroidFacetBuilderPresent

            ``` methodSignature
            public boolean isAndroidFacetBuilderPresent()
            ```

        []{#getAndroidFacet()}

        -   #### getAndroidFacet

            ``` methodSignature
            public Optional<IjModuleAndroidFacet> getAndroidFacet()
            ```

        []{#getSourceFolders()}

        -   #### getSourceFolders

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<IjFolder> getSourceFolders()
            ```

        []{#addExtraLibraryDependency(com.facebook.buck.features.project.intellij.model.IjLibrary)}

        -   #### addExtraLibraryDependency

            ``` methodSignature
            public void addExtraLibraryDependency​(IjLibrary library)
            ```

        []{#getExtraLibraryDependencies()}

        -   #### getExtraLibraryDependencies

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<IjLibrary> getExtraLibraryDependencies()
            ```

        []{#addExtraModuleDependency(java.nio.file.Path)}

        -   #### addExtraModuleDependency

            ``` methodSignature
            public void addExtraModuleDependency​(Path path)
            ```

        []{#getExtraModuleDependencies()}

        -   #### getExtraModuleDependencies

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getExtraModuleDependencies()
            ```

        []{#addNonSourceBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### addNonSourceBuildTarget

            ``` methodSignature
            public void addNonSourceBuildTarget​(BuildTarget buildTarget)
            ```

        []{#getNonSourceBuildTargets()}

        -   #### getNonSourceBuildTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getNonSourceBuildTargets()
            ```

        []{#getTargetsToGeneratedSourcesMap()}

        -   #### getTargetsToGeneratedSourcesMap

            ``` methodSignature
            public Map<BuildTarget,​List<IjFolder>> getTargetsToGeneratedSourcesMap()
            ```

        []{#addGeneratedSourceCodeFolder(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### addGeneratedSourceCodeFolder

            ``` methodSignature
            public void addGeneratedSourceCodeFolder​(BuildTarget buildTarget,
                                                     IjFolder generatedFolder)
            ```

            ::: block
            Add BuildTarget and its associated IjFolder
            :::

        []{#getGeneratedSourceCodeFolders()}

        -   #### getGeneratedSourceCodeFolders

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<IjFolder> getGeneratedSourceCodeFolders()
            ```

        []{#getModuleType()}

        -   #### getModuleType

            ``` methodSignature
            public IjModuleType getModuleType()
            ```

        []{#setModuleType(com.facebook.buck.features.project.intellij.model.IjModuleType)}

        -   #### setModuleType

            ``` methodSignature
            public void setModuleType​(IjModuleType moduleType)
            ```

        []{#getMetaInfDirectory()}

        -   #### getMetaInfDirectory

            ``` methodSignature
            public Optional<Path> getMetaInfDirectory()
            ```

        []{#setMetaInfDirectory(java.nio.file.Path)}

        -   #### setMetaInfDirectory

            ``` methodSignature
            public void setMetaInfDirectory​(Path metaInfDirectory)
            ```

        []{#getJavaLanguageLevel()}

        -   #### getJavaLanguageLevel

            ``` methodSignature
            public Optional<String> getJavaLanguageLevel()
            ```

        []{#setJavaLanguageLevel(java.util.Optional)}

        -   #### setJavaLanguageLevel

            ``` methodSignature
            public void setJavaLanguageLevel​(Optional<String> javaLanguageLevel)
            ```

        []{#getCompilerOutputPath()}

        -   #### getCompilerOutputPath

            ``` methodSignature
            public Optional<Path> getCompilerOutputPath()
            ```

        []{#setCompilerOutputPath(java.util.Optional)}

        -   #### setCompilerOutputPath

            ``` methodSignature
            public void setCompilerOutputPath​(Optional<Path> compilerOutputPath)
            ```

        []{#addSourceFolder(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### addSourceFolder

            ``` methodSignature
            public void addSourceFolder​(IjFolder folder)
            ```

            ::: block
            Adds a source folder to the context. If a folder with the
            same path has already been added the types of the two
            folders will be merged.
            :::

            [Parameters:]{.paramLabel}
            :   `folder` - folder to add/merge.

        []{#addDeps(java.lang.Iterable,com.facebook.buck.features.project.intellij.model.DependencyType)}

        -   #### addDeps

            ``` methodSignature
            public void addDeps​(Iterable<BuildTarget> buildTargets,
                                DependencyType dependencyType)
            ```

        []{#addCompileShadowDep(com.facebook.buck.core.model.BuildTarget)}

        -   #### addCompileShadowDep

            ``` methodSignature
            public void addCompileShadowDep​(BuildTarget buildTarget)
            ```

        []{#addDeps(com.google.common.collect.ImmutableSet,java.lang.Iterable,com.facebook.buck.features.project.intellij.model.DependencyType)}

        -   #### addDeps

            ``` methodSignature
            public void addDeps​(com.google.common.collect.ImmutableSet<Path> sourcePaths,
                                Iterable<BuildTarget> buildTargets,
                                DependencyType dependencyType)
            ```

            ::: block
            Record a dependency on a
            [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model").
            The dependency\'s type will be merged if multiple
            [`TargetNode`](../../../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s
            refer to it or if multiple TargetNodes include sources from
            the same directory.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcePaths` - the
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
                to sources which need this dependency to build. Can be
                empty.
            :   `buildTargets` - the
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                to depend on
            :   `dependencyType` - what is the dependency needed for.

        []{#getDependencies()}

        -   #### getDependencies

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​DependencyType> getDependencies()
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
