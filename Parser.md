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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Interface Parser {#interface-parser .title title="Interface Parser"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface Parser

    ::: block
    High-level build file parsing machinery. Primarily responsible for
    producing a
    [`TargetGraph`](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    based on a set of targets. Caches build rules to minimise the number
    of calls to build file interpreter and processes filesystem events
    to invalidate the cache as files change.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Targe                | `b                    |                       |
        | tGraphCreationResult` | uildTargetGraph​(Parsi |                       |
        |                       | ngContext parsingCont |                       |
        |                       | ext,                  |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSet<Bui |                       |
        |                       | ldTarget> toExplore)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Targe                | `buildTargetGrap      |                       |
        | tGraphCreationResult` | hWithoutTopLevelConfi |                       |
        |                       | gurationTargets​(Parsi |                       |
        |                       | ngContext parsingCont |                       |
        |                       | ext,                  |                       |
        |                       |                       |                       |
        |                       |               Iterabl |                       |
        |                       | e<? extends TargetNod |                       |
        |                       | eSpec> targetNodeSpec |                       |
        |                       | s,                    |                       |
        |                       |                       |                       |
        |                       |             Optional< |                       |
        |                       | TargetConfiguration>  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Targe                | `buildT               |                       |
        | tGraphCreationResult` | argetGraphWithTopLeve |                       |
        |                       | lConfigurationTargets |                       |
        |                       | ​(ParsingContext parsi |                       |
        |                       | ngContext,            |                       |
        |                       |                       |                       |
        |                       |                  Iter |                       |
        |                       | able<? extends Target |                       |
        |                       | NodeSpec> targetNodeS |                       |
        |                       | pecs,                 |                       |
        |                       |                       |                       |
        |                       |             Optional< |                       |
        |                       | TargetConfiguration>  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getAllTarge          |                       |
        | ogle.common.collect.I | tNodes​(PerBuildState  |                       |
        | mmutableList<TargetNo | perBuildState,        |                       |
        | deMaybeIncompatible>` |            Cell cell, |                       |
        |                       |                   Abs |                       |
        |                       | Path buildFile,       |                       |
        |                       |             Optional< |                       |
        |                       | TargetConfiguration>  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getAl                |                       |
        | mmon.collect.Immutabl | lTargetNodesWithTarge |                       |
        | eList<TargetNode<?>>` | tCompatibilityFilteri |                       |
        |                       | ng​(PerBuildState stat |                       |
        |                       | e,                    |                       |
        |                       |                       |                       |
        |                       |           Cell cell,  |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |        AbsPath buildF |                       |
        |                       | ile,                  |                       |
        |                       |                       |                       |
        |                       |             Optional< |                       |
        |                       | TargetConfiguration>  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPe                |                       |
        | PerBuildStateFactory` | rBuildStateFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `DaemonicParserState` | `getPermState()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<?>`       | `getT                 |                       |
        |                       | argetNodeAssertCompat |                       |
        |                       | ible​(ParsingContext p |                       |
        |                       | arsingContext,        |                       |
        |                       |                       |                       |
        |                       |   BuildTarget target, |                       |
        |                       |                       |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<?>`       | `ge                   |                       |
        |                       | tTargetNodeAssertComp |                       |
        |                       | atible​(PerBuildState  |                       |
        |                       | perBuildState,        |                       |
        |                       |                       |                       |
        |                       |   BuildTarget target, |                       |
        |                       |                       |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getTargetNo          |                       |
        | .google.common.util.c | deJobAssertCompatible |                       |
        | oncurrent.ListenableF | ​(PerBuildState perBui |                       |
        | uture<TargetNode<?>>` | ldState,              |                       |
        |                       |                     B |                       |
        |                       | uildTarget target,    |                       |
        |                       |                       |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Sort                 | `g                    | ::: block             |
        | edMap<String,​Object>` | etTargetNodeRawAttrib | [Deprecate            |
        |                       | utes​(ParsingContext p | d.]{.deprecatedLabel} |
        |                       | arsingContext,        |                       |
        |                       |                     T | :                     |
        |                       | argetNode<?> targetNo | :: deprecationComment |
        |                       | de,                   | Prefer                |
        |                       |          DependencySt | [`getTargetNodeR      |
        |                       | ack dependencyStack)` | awAttributes(PerBuild |
        |                       |                       | State, Cell, TargetNo |
        |                       |                       | de,      DependencySt |
        |                       |                       | ack)`](#getTargetNode |
        |                       |                       | RawAttributes(com.fac |
        |                       |                       | ebook.buck.parser.Per |
        |                       |                       | BuildState,com.facebo |
        |                       |                       | ok.buck.core.cell.Cel |
        |                       |                       | l,com.facebook.buck.c |
        |                       |                       | ore.model.targetgraph |
        |                       |                       | .TargetNode,com.faceb |
        |                       |                       | ook.buck.core.excepti |
        |                       |                       | ons.DependencyStack)) |
        |                       |                       | and reusing a         |
        |                       |                       | PerBuildState         |
        |                       |                       | instance, especially  |
        |                       |                       | when calling in a     |
        |                       |                       | loop.                 |
        |                       |                       | :::                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Sort                 | `getTarg              |                       |
        | edMap<String,​Object>` | etNodeRawAttributes​(P |                       |
        |                       | erBuildState state,   |                       |
        |                       |                       |                       |
        |                       |     Cell cell,        |                       |
        |                       |                     T |                       |
        |                       | argetNode<?> targetNo |                       |
        |                       | de,                   |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getTargetNodeRawAtt  |                       |
        | mon.util.concurrent.L | ributesJob​(PerBuildSt |                       |
        | istenableFuture<Sorte | ate state,            |                       |
        | dMap<String,​Object>>` |                    Ce |                       |
        |                       | ll cell,              |                       |
        |                       |                  Targ |                       |
        |                       | etNode<?> targetNode, |                       |
        |                       |                       |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `resolveTarg          |                       |
        | e.common.collect.Immu | etSpecs​(ParsingContex |                       |
        | tableList<com.google. | t parsingContext,     |                       |
        | common.collect.Immuta |                Iterab |                       |
        | bleSet<BuildTarget>>` | le<? extends TargetNo |                       |
        |                       | deSpec> specs,        |                       |
        |                       |             Optional< |                       |
        |                       | TargetConfiguration>  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPermState()}

        -   #### getPermState

            ``` methodSignature
            DaemonicParserState getPermState()
            ```

        []{#getPerBuildStateFactory()}

        -   #### getPerBuildStateFactory

            ``` methodSignature
            PerBuildStateFactory getPerBuildStateFactory()
            ```

        []{#getTargetNodeAssertCompatible(com.facebook.buck.parser.ParsingContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetNodeAssertCompatible

            ``` methodSignature
            TargetNode<?> getTargetNodeAssertCompatible​(ParsingContext parsingContext,
                                                        BuildTarget target,
                                                        DependencyStack dependencyStack)
                                                 throws BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#getAllTargetNodes(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath,java.util.Optional)}

        -   #### getAllTargetNodes

            ``` methodSignature
            com.google.common.collect.ImmutableList<TargetNodeMaybeIncompatible> getAllTargetNodes​(PerBuildState perBuildState,
                                                                                                   Cell cell,
                                                                                                   AbsPath buildFile,
                                                                                                   Optional<TargetConfiguration> targetConfiguration)
                                                                                            throws BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#getAllTargetNodesWithTargetCompatibilityFiltering(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath,java.util.Optional)}

        -   #### getAllTargetNodesWithTargetCompatibilityFiltering

            ``` methodSignature
            com.google.common.collect.ImmutableList<TargetNode<?>> getAllTargetNodesWithTargetCompatibilityFiltering​(PerBuildState state,
                                                                                                                     Cell cell,
                                                                                                                     AbsPath buildFile,
                                                                                                                     Optional<TargetConfiguration> targetConfiguration)
                                                                                                              throws BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#getTargetNodeAssertCompatible(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetNodeAssertCompatible

            ``` methodSignature
            TargetNode<?> getTargetNodeAssertCompatible​(PerBuildState perBuildState,
                                                        BuildTarget target,
                                                        DependencyStack dependencyStack)
                                                 throws BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#getTargetNodeJobAssertCompatible(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetNodeJobAssertCompatible

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<TargetNode<?>> getTargetNodeJobAssertCompatible​(PerBuildState perBuildState,
                                                                                                               BuildTarget target,
                                                                                                               DependencyStack dependencyStack)
                                                                                                        throws BuildTargetException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildTargetException`

        []{#getTargetNodeRawAttributes(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetNodeRawAttributes

            ``` methodSignature
            @Nullable
            SortedMap<String,​Object> getTargetNodeRawAttributes​(PerBuildState state,
                                                                      Cell cell,
                                                                      TargetNode<?> targetNode,
                                                                      DependencyStack dependencyStack)
                                                               throws BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#getTargetNodeRawAttributesJob(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetNodeRawAttributesJob

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<SortedMap<String,​Object>> getTargetNodeRawAttributesJob​(PerBuildState state,
                                                                                                                             Cell cell,
                                                                                                                             TargetNode<?> targetNode,
                                                                                                                             DependencyStack dependencyStack)
                                                                                                                      throws BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#getTargetNodeRawAttributes(com.facebook.buck.parser.ParsingContext,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetNodeRawAttributes

            ``` methodSignature
            @Nullable
            @Deprecated
            SortedMap<String,​Object> getTargetNodeRawAttributes​(ParsingContext parsingContext,
                                                                      TargetNode<?> targetNode,
                                                                      DependencyStack dependencyStack)
                                                               throws BuildFileParseException
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}

            ::: deprecationComment
            Prefer
            [`getTargetNodeRawAttributes(PerBuildState, Cell, TargetNode,      DependencyStack)`](#getTargetNodeRawAttributes(com.facebook.buck.parser.PerBuildState,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.exceptions.DependencyStack))
            and reusing a PerBuildState instance, especially when
            calling in a loop.
            :::
            :::

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`

        []{#buildTargetGraph(com.facebook.buck.parser.ParsingContext,com.google.common.collect.ImmutableSet)}

        -   #### buildTargetGraph

            ``` methodSignature
            TargetGraphCreationResult buildTargetGraph​(ParsingContext parsingContext,
                                                       com.google.common.collect.ImmutableSet<BuildTarget> toExplore)
                                                throws IOException,
                                                       InterruptedException,
                                                       BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
            :   `BuildFileParseException`

        []{#buildTargetGraphWithoutTopLevelConfigurationTargets(com.facebook.buck.parser.ParsingContext,java.lang.Iterable,java.util.Optional)}

        -   #### buildTargetGraphWithoutTopLevelConfigurationTargets

            ``` methodSignature
            TargetGraphCreationResult buildTargetGraphWithoutTopLevelConfigurationTargets​(ParsingContext parsingContext,
                                                                                          Iterable<? extends TargetNodeSpec> targetNodeSpecs,
                                                                                          Optional<TargetConfiguration> targetConfiguration)
                                                                                   throws BuildFileParseException,
                                                                                          IOException,
                                                                                          InterruptedException
            ```

            [Parameters:]{.paramLabel}
            :   `targetNodeSpecs` - the specs representing the build
                targets to generate a target graph for.
            :   `targetConfiguration` -

            [Returns:]{.returnLabel}
            :   the target graph containing the build targets and their
                related targets.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `IOException`
            :   `InterruptedException`

        []{#buildTargetGraphWithTopLevelConfigurationTargets(com.facebook.buck.parser.ParsingContext,java.lang.Iterable,java.util.Optional)}

        -   #### buildTargetGraphWithTopLevelConfigurationTargets

            ``` methodSignature
            TargetGraphCreationResult buildTargetGraphWithTopLevelConfigurationTargets​(ParsingContext parsingContext,
                                                                                       Iterable<? extends TargetNodeSpec> targetNodeSpecs,
                                                                                       Optional<TargetConfiguration> targetConfiguration)
                                                                                throws BuildFileParseException,
                                                                                       IOException,
                                                                                       InterruptedException
            ```

            [Parameters:]{.paramLabel}
            :   `targetNodeSpecs` - the specs representing the build
                targets to generate a target graph for.
            :   `targetConfiguration` -

            [Returns:]{.returnLabel}
            :   the target graph containing the build targets and their
                related targets.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `IOException`
            :   `InterruptedException`

        []{#resolveTargetSpecs(com.facebook.buck.parser.ParsingContext,java.lang.Iterable,java.util.Optional)}

        -   #### resolveTargetSpecs

            ``` methodSignature
            com.google.common.collect.ImmutableList<com.google.common.collect.ImmutableSet<BuildTarget>> resolveTargetSpecs​(ParsingContext parsingContext,
                                                                                                                            Iterable<? extends TargetNodeSpec> specs,
                                                                                                                            Optional<TargetConfiguration> targetConfiguration)
                                                                                                                     throws BuildFileParseException,
                                                                                                                            InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
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
