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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class UnconfiguredTargetNodeToTargetNodeFactory {#class-unconfiguredtargetnodetotargetnodefactory .title title="Class UnconfiguredTargetNodeToTargetNodeFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.UnconfiguredTargetNodeToTargetNodeFactory

::: description
-   

    All Implemented Interfaces:
    :   `ParserTargetNodeFromUnconfiguredTargetNodeFactory`

    ------------------------------------------------------------------------

        public class UnconfiguredTargetNodeToTargetNodeFactory
        extends Object
        implements ParserTargetNodeFromUnconfiguredTargetNodeFactory

    ::: block
    Creates
    [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    from
    [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `UnconfiguredTargetNodeToTargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,                                          KnownRuleTypesProvider knownRuleTypesProvider,                                          ConstructorArgMarshaller marshaller,                                          TargetNodeFactory targetNodeFactory,                                          PackageBoundaryChecker packageBoundaryChecker,                                          TargetNodeListener<TargetNode<?>> nodeListener,                                          SelectorListResolver selectorListResolver,                                          TargetPlatformResolver targetPlatformResolver,                                          TargetConfigurationTransformer targetConfigurationTransformer,                                          TargetConfiguration hostConfiguration,                                          BuckConfig buckConfig,                                          Optional<ConfigurationRuleRegistry> configurationRuleRegistry)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type               Method                                                                                                                                                                                                                                                                                                                                Description
          ------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetNodeMaybeIncompatible`   `createTargetNode​(Cell cell,                 AbsPath buildFile,                 BuildTarget target,                 DependencyStack dependencyStack,                 UnconfiguredTargetNode unconfiguredTargetNode,                 java.util.function.Function<SimplePerfEvent.PerfEventId,​SimplePerfEvent.Scope> perfEventScope)`    

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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,com.facebook.buck.rules.coercer.ConstructorArgMarshaller,com.facebook.buck.core.model.targetgraph.impl.TargetNodeFactory,com.facebook.buck.parser.PackageBoundaryChecker,com.facebook.buck.parser.TargetNodeListener,com.facebook.buck.core.select.SelectorListResolver,com.facebook.buck.core.model.platform.TargetPlatformResolver,com.facebook.buck.core.model.TargetConfigurationTransformer,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.config.BuckConfig,java.util.Optional)}

        -   #### UnconfiguredTargetNodeToTargetNodeFactory

                public UnconfiguredTargetNodeToTargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,
                                                                 KnownRuleTypesProvider knownRuleTypesProvider,
                                                                 ConstructorArgMarshaller marshaller,
                                                                 TargetNodeFactory targetNodeFactory,
                                                                 PackageBoundaryChecker packageBoundaryChecker,
                                                                 TargetNodeListener<TargetNode<?>> nodeListener,
                                                                 SelectorListResolver selectorListResolver,
                                                                 TargetPlatformResolver targetPlatformResolver,
                                                                 TargetConfigurationTransformer targetConfigurationTransformer,
                                                                 TargetConfiguration hostConfiguration,
                                                                 BuckConfig buckConfig,
                                                                 Optional<ConfigurationRuleRegistry> configurationRuleRegistry)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createTargetNode(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.model.targetgraph.raw.UnconfiguredTargetNode,java.util.function.Function)}

        -   #### createTargetNode

            ``` methodSignature
            public TargetNodeMaybeIncompatible createTargetNode​(Cell cell,
                                                                AbsPath buildFile,
                                                                BuildTarget target,
                                                                DependencyStack dependencyStack,
                                                                UnconfiguredTargetNode unconfiguredTargetNode,
                                                                java.util.function.Function<SimplePerfEvent.PerfEventId,​SimplePerfEvent.Scope> perfEventScope)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createTargetNode` in
                interface `ParserTargetNodeFromUnconfiguredTargetNodeFactory`
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
