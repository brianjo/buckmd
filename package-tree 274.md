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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.parser {#hierarchy-for-package-com.facebook.buck.parser .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.parser.[[ParseEvent]{.typeNameLink}](ParseEvent.html "class in com.facebook.buck.parser")
            (implements
            com.facebook.buck.event.[LeafEvent](../event/LeafEvent.html "interface in com.facebook.buck.event"),
            com.facebook.buck.event.[WorkAdvanceEvent](../event/WorkAdvanceEvent.html "interface in com.facebook.buck.event"))
            -   com.facebook.buck.parser.[[ParseEvent.Finished]{.typeNameLink}](ParseEvent.Finished.html "class in com.facebook.buck.parser")
            -   com.facebook.buck.parser.[[ParseEvent.Started]{.typeNameLink}](ParseEvent.Started.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[BuildTargetRawNodeParsePipeline]{.typeNameLink}](BuildTargetRawNodeParsePipeline.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[BuildTargetParsePipeline](BuildTargetParsePipeline.html "interface in com.facebook.buck.parser")\<T\>)
    -   com.facebook.buck.parser.[[BuiltTargetVerifier]{.typeNameLink}](BuiltTargetVerifier.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[ConcurrentProjectBuildFileParser]{.typeNameLink}](ConcurrentProjectBuildFileParser.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.api.[ProjectBuildFileParser](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api"))
    -   com.facebook.buck.parser.[[DaemonicParserState]{.typeNameLink}](DaemonicParserState.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[DefaultProjectBuildFileParserFactory]{.typeNameLink}](DefaultProjectBuildFileParserFactory.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[ProjectBuildFileParserFactory](ProjectBuildFileParserFactory.html "interface in com.facebook.buck.parser"))
    -   com.facebook.buck.parser.[[DefaultSelectableConfigurationContext]{.typeNameLink}](DefaultSelectableConfigurationContext.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.core.rules.configsetting.[ConfigSettingSelectableConfigurationContext](../core/rules/configsetting/ConfigSettingSelectableConfigurationContext.html "interface in com.facebook.buck.core.rules.configsetting"))
    -   com.facebook.buck.parser.[[DefaultUnconfiguredTargetNodeFactory]{.typeNameLink}](DefaultUnconfiguredTargetNodeFactory.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[UnconfiguredTargetNodeFactory](UnconfiguredTargetNodeFactory.html "interface in com.facebook.buck.parser"))
    -   com.facebook.buck.parser.[[GenericFileParsePipeline]{.typeNameLink}](GenericFileParsePipeline.html "class in com.facebook.buck.parser")\<T\>
        (implements
        com.facebook.buck.parser.[FileParsePipeline](FileParsePipeline.html "interface in com.facebook.buck.parser")\<T\>)
        -   com.facebook.buck.parser.[[BuildFileRawNodeParsePipeline]{.typeNameLink}](BuildFileRawNodeParsePipeline.html "class in com.facebook.buck.parser")
        -   com.facebook.buck.parser.[[PackageFileParsePipeline]{.typeNameLink}](PackageFileParsePipeline.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[HybridProjectBuildFileParser]{.typeNameLink}](HybridProjectBuildFileParser.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.api.[ProjectBuildFileParser](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api"))
    -   com.facebook.buck.parser.ImmutableParsingContext.Builder
        -   com.facebook.buck.parser.[[ParsingContext.Builder]{.typeNameLink}](ParsingContext.Builder.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[InternalTargetAttributeNames]{.typeNameLink}](InternalTargetAttributeNames.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[LabelCache]{.typeNameLink}](LabelCache.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[MetaRules]{.typeNameLink}](MetaRules.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[NoopPackageBoundaryChecker]{.typeNameLink}](NoopPackageBoundaryChecker.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[PackageBoundaryChecker](PackageBoundaryChecker.html "interface in com.facebook.buck.parser"))
    -   com.facebook.buck.parser.[[PackageFactory]{.typeNameLink}](PackageFactory.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[PackageFileParserFactory]{.typeNameLink}](PackageFileParserFactory.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[FileParserFactory](FileParserFactory.html "interface in com.facebook.buck.parser")\<T\>)
    -   com.facebook.buck.parser.[[ParserFactory]{.typeNameLink}](ParserFactory.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[ParserMessages]{.typeNameLink}](ParserMessages.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[ParserPythonInterpreterProvider]{.typeNameLink}](ParserPythonInterpreterProvider.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[ParsingContext]{.typeNameLink}](ParsingContext.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[PerBuildState]{.typeNameLink}](PerBuildState.html "class in com.facebook.buck.parser")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   com.facebook.buck.parser.[[PerBuildStateFactory]{.typeNameLink}](PerBuildStateFactory.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[PythonDslProjectBuildFileParser]{.typeNameLink}](PythonDslProjectBuildFileParser.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.api.[ProjectBuildFileParser](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api"))
    -   com.facebook.buck.parser.[[TargetSpecResolver]{.typeNameLink}](TargetSpecResolver.html "class in com.facebook.buck.parser")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.lang.[[RuntimeException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}
                -   com.facebook.buck.core.exceptions.[[HumanReadableException]{.typeNameLink}](../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")
                    (implements
                    com.facebook.buck.core.exceptions.[ExceptionWithHumanReadableMessage](../core/exceptions/ExceptionWithHumanReadableMessage.html "interface in com.facebook.buck.core.exceptions"))
                    -   com.facebook.buck.parser.[[UnexpectedFlavorException]{.typeNameLink}](UnexpectedFlavorException.html "class in com.facebook.buck.parser")
    -   com.facebook.buck.parser.[[ThrowingPackageBoundaryChecker]{.typeNameLink}](ThrowingPackageBoundaryChecker.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[PackageBoundaryChecker](PackageBoundaryChecker.html "interface in com.facebook.buck.parser"))
    -   com.facebook.buck.parser.[[UnconfiguredTargetNodePipeline]{.typeNameLink}](UnconfiguredTargetNodePipeline.html "class in com.facebook.buck.parser")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   com.facebook.buck.parser.[[UnconfiguredTargetNodeToTargetNodeFactory]{.typeNameLink}](UnconfiguredTargetNodeToTargetNodeFactory.html "class in com.facebook.buck.parser")
        (implements
        com.facebook.buck.parser.[ParserTargetNodeFromUnconfiguredTargetNodeFactory](ParserTargetNodeFromUnconfiguredTargetNodeFactory.html "interface in com.facebook.buck.parser"))
    -   com.facebook.buck.parser.[[UnconfiguredTargetNodeToTargetNodeParsePipeline]{.typeNameLink}](UnconfiguredTargetNodeToTargetNodeParsePipeline.html "class in com.facebook.buck.parser")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   com.facebook.buck.parser.[[UnflavoredBuildTargetFactory]{.typeNameLink}](UnflavoredBuildTargetFactory.html "class in com.facebook.buck.parser")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.parser.[[BuildTargetParsePipeline]{.typeNameLink}](BuildTargetParsePipeline.html "interface in com.facebook.buck.parser")\<T\>
    -   com.facebook.buck.parser.[[FileParsePipeline]{.typeNameLink}](FileParsePipeline.html "interface in com.facebook.buck.parser")\<T\>
-   com.facebook.buck.parser.[[FileParserFactory]{.typeNameLink}](FileParserFactory.html "interface in com.facebook.buck.parser")\<T\>
    -   com.facebook.buck.parser.[[ProjectBuildFileParserFactory]{.typeNameLink}](ProjectBuildFileParserFactory.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[PackageBoundaryChecker]{.typeNameLink}](PackageBoundaryChecker.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[Parser]{.typeNameLink}](Parser.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[ParserTargetNodeFromAttrMapFactory]{.typeNameLink}](ParserTargetNodeFromAttrMapFactory.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[ParserTargetNodeFromUnconfiguredTargetNodeFactory]{.typeNameLink}](ParserTargetNodeFromUnconfiguredTargetNodeFactory.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[TargetNodeListener]{.typeNameLink}](TargetNodeListener.html "interface in com.facebook.buck.parser")\<T\>
-   com.facebook.buck.parser.[[TargetSpecResolver.FlavorEnhancer]{.typeNameLink}](TargetSpecResolver.FlavorEnhancer.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[TargetSpecResolver.TargetNodeFilterForSpecResolver]{.typeNameLink}](TargetSpecResolver.TargetNodeFilterForSpecResolver.html "interface in com.facebook.buck.parser")
-   com.facebook.buck.parser.[[UnconfiguredTargetNodeFactory]{.typeNameLink}](UnconfiguredTargetNodeFactory.html "interface in com.facebook.buck.parser")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.parser.[[SpeculativeParsing]{.typeNameLink}](SpeculativeParsing.html "enum in com.facebook.buck.parser")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
