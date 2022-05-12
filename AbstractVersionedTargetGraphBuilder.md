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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Class AbstractVersionedTargetGraphBuilder {#class-abstractversionedtargetgraphbuilder .title title="Class AbstractVersionedTargetGraphBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.versions.AbstractVersionedTargetGraphBuilder

::: description
-   

    All Implemented Interfaces:
    :   `VersionedTargetGraphBuilder`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AsyncVersionedTargetGraphBuilder`

    ------------------------------------------------------------------------

        public abstract class AbstractVersionedTargetGraphBuilder
        extends Object
        implements VersionedTargetGraphBuilder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                       Field                                    Description
          --------------------------------------- ---------------------------------------- -------------
          `protected long`                        `timeout`                                 
          `protected TimeUnit`                    `timeUnit`                                
          `protected TypeCoercerFactory`          `typeCoercerFactory`                      
          `protected TargetGraphCreationResult`   `unversionedTargetGraphCreationResult`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          -------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AbstractVersionedTargetGraphBuilder​(TypeCoercerFactory typeCoercerFactory,                                    UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                                    TargetGraphCreationResult unversionedTargetGraphCreationResult,                                    long timeout,                                    TimeUnit timeUnit,                                    Cells cells)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `getNode              |                       |
        | tected TargetNode<?>` | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Opt        | `getNodeOptional      |                       |
        | ional<TargetNode<?>>` | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getTargetNodeTransl  |                       |
        | TargetNodeTranslator` | ator​(TargetNode<?> ro |                       |
        |                       | ot,                   |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ap<BuildTarget,​Versio |                       |
        |                       | n> selectedVersions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected O          | `getTranslateBuildTa  |                       |
        | ptional<BuildTarget>` | rget​(TargetNode<?> no |                       |
        |                       | de,                   |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ap<BuildTarget,​Versio |                       |
        |                       | n> selectedVersions)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstra     | `getVersionInfo       | ::: block             |
        | ct com.facebook.buck. | ​(TargetNode<?> node)` | Get/cache the         |
        | versions.VersionInfo` |                       | transitive version    |
        |                       |                       | info for this node.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `res                  |                       |
        | tected TargetNode<?>` | olveVersions​(TargetNo |                       |
        |                       | de<?> node,           |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ap<BuildTarget,​Versio |                       |
        |                       | n> selectedVersions)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.versions.VersionedTargetGraphBuilder}

            ### Methods inherited from interface com.facebook.buck.versions.[VersionedTargetGraphBuilder](VersionedTargetGraphBuilder.html "interface in com.facebook.buck.versions")

            `build`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#typeCoercerFactory}

        -   #### typeCoercerFactory

                protected final TypeCoercerFactory typeCoercerFactory

        []{#unversionedTargetGraphCreationResult}

        -   #### unversionedTargetGraphCreationResult

                protected final TargetGraphCreationResult unversionedTargetGraphCreationResult

        []{#timeout}

        -   #### timeout

                protected final long timeout

        []{#timeUnit}

        -   #### timeUnit

                protected final TimeUnit timeUnit
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,long,java.util.concurrent.TimeUnit,com.facebook.buck.core.cell.Cells)}

        -   #### AbstractVersionedTargetGraphBuilder

                protected AbstractVersionedTargetGraphBuilder​(TypeCoercerFactory typeCoercerFactory,
                                                              UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                              TargetGraphCreationResult unversionedTargetGraphCreationResult,
                                                              long timeout,
                                                              TimeUnit timeUnit,
                                                              Cells cells)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNode(com.facebook.buck.core.model.BuildTarget)}

        -   #### getNode

            ``` methodSignature
            protected TargetNode<?> getNode​(BuildTarget target)
            ```

        []{#getNodeOptional(com.facebook.buck.core.model.BuildTarget)}

        -   #### getNodeOptional

            ``` methodSignature
            protected Optional<TargetNode<?>> getNodeOptional​(BuildTarget target)
            ```

        []{#resolveVersions(com.facebook.buck.core.model.targetgraph.TargetNode,com.google.common.collect.ImmutableMap)}

        -   #### resolveVersions

            ``` methodSignature
            protected final TargetNode<?> resolveVersions​(TargetNode<?> node,
                                                          com.google.common.collect.ImmutableMap<BuildTarget,​Version> selectedVersions)
            ```

        []{#getVersionInfo(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getVersionInfo

            ``` methodSignature
            protected abstract com.facebook.buck.versions.VersionInfo getVersionInfo​(TargetNode<?> node)
            ```

            ::: block
            Get/cache the transitive version info for this node.
            :::

        []{#getTranslateBuildTarget(com.facebook.buck.core.model.targetgraph.TargetNode,com.google.common.collect.ImmutableMap)}

        -   #### getTranslateBuildTarget

            ``` methodSignature
            protected final Optional<BuildTarget> getTranslateBuildTarget​(TargetNode<?> node,
                                                                          com.google.common.collect.ImmutableMap<BuildTarget,​Version> selectedVersions)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                to use in the resolved target graph, formed by adding a
                flavor generated from the given version selections.

        []{#getTargetNodeTranslator(com.facebook.buck.core.model.targetgraph.TargetNode,com.google.common.collect.ImmutableMap)}

        -   #### getTargetNodeTranslator

            ``` methodSignature
            protected TargetNodeTranslator getTargetNodeTranslator​(TargetNode<?> root,
                                                                   com.google.common.collect.ImmutableMap<BuildTarget,​Version> selectedVersions)
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
