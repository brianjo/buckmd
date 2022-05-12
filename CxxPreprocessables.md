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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxPreprocessables {#class-cxxpreprocessables .title title="Class CxxPreprocessables"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxPreprocessables

::: description
-   

    ------------------------------------------------------------------------

        public class CxxPreprocessables
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                              Description
          ------------------- ---------------------------------- -------------
          `static class `     `CxxPreprocessables.IncludeType`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static CxxPrepr      | `addHeaderSymlinkTre  |                       |
        | ocessorInput.Builder` | e​(CxxPreprocessorInpu |                       |
        |                       | t.Builder builder,    |                       |
        |                       |                   Bui |                       |
        |                       | ldTarget target,      |                       |
        |                       |                 Actio |                       |
        |                       | nGraphBuilder graphBu |                       |
        |                       | ilder,                |                       |
        |                       |       CxxPlatform pla |                       |
        |                       | tform,                |                       |
        |                       |       HeaderVisibilit |                       |
        |                       | y headerVisibility,   |                       |
        |                       |                    Cx |                       |
        |                       | xPreprocessables.Incl |                       |
        |                       | udeType includeType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `createHeaderSy       | ::: block             |
        | ic HeaderSymlinkTree` | mlinkTreeBuildRule​(Bu | Build the             |
        |                       | ildTarget target,     | [`HeaderSymlin        |
        |                       |                       | kTree`](toolchain/Hea |
        |                       |         ProjectFilesy | derSymlinkTree.html " |
        |                       | stem filesystem,      | class in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |        Path root,     | rule using the        |
        |                       |                       | original build params |
        |                       |         com.google.co | from a target node.   |
        |                       | mmon.collect.Immutabl | :::                   |
        |                       | eMap<Path,​SourcePath> |                       |
        |                       |  links,               |                       |
        |                       |                    He |                       |
        |                       | aderMode headerMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getCxxPrepro         | ::: block             |
        | CxxPreprocessorInput` | cessorInput​(BuildTarg | Builds a              |
        |                       | et buildTarget,       | [`CxxPreprocessorInpu |
        |                       |                   Act | t`](CxxPreprocessorIn |
        |                       | ionGraphBuilder graph | put.html "class in co |
        |                       | Builder,              | m.facebook.buck.cxx") |
        |                       |            boolean ha | for a rule.           |
        |                       | sHeaderSymlinkTree,   | :::                   |
        |                       |                       |                       |
        |                       |  CxxPlatform platform |                       |
        |                       | ,                     |                       |
        |                       |     HeaderVisibility  |                       |
        |                       | headerVisibility,     |                       |
        |                       |                     C |                       |
        |                       | xxPreprocessables.Inc |                       |
        |                       | ludeType includeType, |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.Multimap<CxxS |                       |
        |                       | ource.Type,​String> ex |                       |
        |                       | portedPreprocessorFla |                       |
        |                       | gs,                   |                       |
        |                       |       Iterable<Framew |                       |
        |                       | orkPath> frameworks)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Collection<C  | `getTransitiveCxx     | ::: block             |
        | xxPreprocessorInput>` | PreprocessorInput​(Cxx | Find and return the   |
        |                       | Platform cxxPlatform, | [`CxxPreprocessorInpu |
        |                       |                       | t`](CxxPreprocessorIn |
        |                       |              ActionGr | put.html "class in co |
        |                       | aphBuilder graphBuild | m.facebook.buck.cxx") |
        |                       | er,                   | objects from          |
        |                       |                 Itera | [`CxxPreprocessorDep` |
        |                       | ble<? extends CxxPrep | ](CxxPreprocessorDep. |
        |                       | rocessorDep> inputs)` | html "interface in co |
        |                       |                       | m.facebook.buck.cxx") |
        |                       |                       | found.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Collection<C  | `getTrans             | ::: block             |
        | xxPreprocessorInput>` | itiveCxxPreprocessorI | Find and return the   |
        |                       | nputFromDeps​(CxxPlatf | [`CxxPreprocessorInpu |
        |                       | orm cxxPlatform,      | t`](CxxPreprocessorIn |
        |                       |                       | put.html "class in co |
        |                       |                 Actio | m.facebook.buck.cxx") |
        |                       | nGraphBuilder graphBu | objects from          |
        |                       | ilder,                | [`CxxPreprocessorDep` |
        |                       |                       | ](CxxPreprocessorDep. |
        |                       |       Iterable<? exte | html "interface in co |
        |                       | nds BuildRule> deps)` | m.facebook.buck.cxx") |
        |                       |                       | found from a list of  |
        |                       |                       | all deps.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `resolveHea           | ::: block             |
        | static com.google.com | derMap​(Path basePath, | Resolve the map of    |
        | mon.collect.Immutable |                  com. | name to               |
        | Map<Path,​SourcePath>` | google.common.collect | [`SourcePath`](       |
        |                       | .ImmutableMap<String, | ../core/sourcepath/So |
        |                       | ​SourcePath> headers)` | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | to a map of full      |
        |                       |                       | header name to        |
        |                       |                       | [`SourcePath`](.      |
        |                       |                       | ./core/sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath"). |
        |                       |                       | :::                   |
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

        []{#resolveHeaderMap(java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### resolveHeaderMap

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> resolveHeaderMap​(Path basePath,
                                                                                                         com.google.common.collect.ImmutableMap<String,​SourcePath> headers)
            ```

            ::: block
            Resolve the map of name to
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            to a map of full header name to
            [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath").
            :::

        []{#getTransitiveCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable)}

        -   #### getTransitiveCxxPreprocessorInput

            ``` methodSignature
            public static Collection<CxxPreprocessorInput> getTransitiveCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                                             ActionGraphBuilder graphBuilder,
                                                                                             Iterable<? extends CxxPreprocessorDep> inputs)
            ```

            ::: block
            Find and return the
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            objects from
            [`CxxPreprocessorDep`](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")
            found.
            :::

        []{#getTransitiveCxxPreprocessorInputFromDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable)}

        -   #### getTransitiveCxxPreprocessorInputFromDeps

            ``` methodSignature
            public static Collection<CxxPreprocessorInput> getTransitiveCxxPreprocessorInputFromDeps​(CxxPlatform cxxPlatform,
                                                                                                     ActionGraphBuilder graphBuilder,
                                                                                                     Iterable<? extends BuildRule> deps)
            ```

            ::: block
            Find and return the
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            objects from
            [`CxxPreprocessorDep`](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")
            found from a list of all deps.
            :::

        []{#createHeaderSymlinkTreeBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.HeaderMode)}

        -   #### createHeaderSymlinkTreeBuildRule

            ``` methodSignature
            public static HeaderSymlinkTree createHeaderSymlinkTreeBuildRule​(BuildTarget target,
                                                                             ProjectFilesystem filesystem,
                                                                             Path root,
                                                                             com.google.common.collect.ImmutableMap<Path,​SourcePath> links,
                                                                             HeaderMode headerMode)
            ```

            ::: block
            Build the
            [`HeaderSymlinkTree`](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain")
            rule using the original build params from a target node. In
            particular, make sure to drop all dependencies from the
            original build rule params, as these are modeled via
            [`CxxPreprocessAndCompile`](CxxPreprocessAndCompile.html "class in com.facebook.buck.cxx").
            :::

        []{#addHeaderSymlinkTree(com.facebook.buck.cxx.CxxPreprocessorInput.Builder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.HeaderVisibility,com.facebook.buck.cxx.CxxPreprocessables.IncludeType)}

        -   #### addHeaderSymlinkTree

            ``` methodSignature
            public static CxxPreprocessorInput.Builder addHeaderSymlinkTree​(CxxPreprocessorInput.Builder builder,
                                                                            BuildTarget target,
                                                                            ActionGraphBuilder graphBuilder,
                                                                            CxxPlatform platform,
                                                                            HeaderVisibility headerVisibility,
                                                                            CxxPreprocessables.IncludeType includeType)
            ```

            [Returns:]{.returnLabel}
            :   adds a the header
                [`SymlinkTree`](../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
                for the given rule to the
                [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx").

        []{#getCxxPreprocessorInput(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,boolean,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.HeaderVisibility,com.facebook.buck.cxx.CxxPreprocessables.IncludeType,com.google.common.collect.Multimap,java.lang.Iterable)}

        -   #### getCxxPreprocessorInput

            ``` methodSignature
            public static CxxPreprocessorInput getCxxPreprocessorInput​(BuildTarget buildTarget,
                                                                       ActionGraphBuilder graphBuilder,
                                                                       boolean hasHeaderSymlinkTree,
                                                                       CxxPlatform platform,
                                                                       HeaderVisibility headerVisibility,
                                                                       CxxPreprocessables.IncludeType includeType,
                                                                       com.google.common.collect.Multimap<CxxSource.Type,​String> exportedPreprocessorFlags,
                                                                       Iterable<FrameworkPath> frameworks)
            ```

            ::: block
            Builds a
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            for a rule.
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
