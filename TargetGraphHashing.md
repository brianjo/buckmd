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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.impl](package-summary.html)
:::

## Class TargetGraphHashing {#class-targetgraphhashing .title title="Class TargetGraphHashing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.impl.TargetGraphHashing

::: description
-   

    ------------------------------------------------------------------------

        public class TargetGraphHashing
        extends Object

    ::: block
    Utility class to calculate hash codes for build targets in a
    [`TargetGraph`](../TargetGraph.html "class in com.facebook.buck.core.model.targetgraph").
    A build target\'s hash code is guaranteed to change if the build
    target or any of its dependencies change, including the contents of
    all input files to the target and its dependencies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetGraphHashing​(BuckEventBus eventBus,                   TargetGraph targetGraph,                   FileHashLoader fileHashLoader,                   Iterable<TargetNode<?>> roots,                   com.google.common.util.concurrent.ListeningExecutorService executor,                   RuleKeyConfiguration ruleKeyConfiguration,                   java.util.function.Function<TargetNode<?>,​com.google.common.util.concurrent.ListenableFuture<?>> targetNodeRawAttributesProvider,                   com.google.common.hash.HashFunction hashFunction)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `hashTargetGraph()`   | ::: block             |
        | com.google.common.col |                       | Given a               |
        | lect.ImmutableMap<Bui |                       | [`Ta                  |
        | ldTarget,​com.google.c |                       | rgetGraph`](../Target |
        | ommon.hash.HashCode>` |                       | Graph.html "class in  |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.model.targetgraph") |
        |                       |                       | and any number of     |
        |                       |                       | root nodes to         |
        |                       |                       | traverse, returns a   |
        |                       |                       | map of                |
        |                       |                       | `  (Bu                |
        |                       |                       | ildTarget, HashCode)` |
        |                       |                       | pairs for all root    |
        |                       |                       | build targets and     |
        |                       |                       | their dependencies.   |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.util.hashing.FileHashLoader,java.lang.Iterable,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,java.util.function.Function,com.google.common.hash.HashFunction)}

        -   #### TargetGraphHashing

                public TargetGraphHashing​(BuckEventBus eventBus,
                                          TargetGraph targetGraph,
                                          FileHashLoader fileHashLoader,
                                          Iterable<TargetNode<?>> roots,
                                          com.google.common.util.concurrent.ListeningExecutorService executor,
                                          RuleKeyConfiguration ruleKeyConfiguration,
                                          java.util.function.Function<TargetNode<?>,​com.google.common.util.concurrent.ListenableFuture<?>> targetNodeRawAttributesProvider,
                                          com.google.common.hash.HashFunction hashFunction)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#hashTargetGraph()}

        -   #### hashTargetGraph

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​com.google.common.hash.HashCode> hashTargetGraph()
                                                                                                                      throws InterruptedException
            ```

            ::: block
            Given a
            [`TargetGraph`](../TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
            and any number of root nodes to traverse, returns a map of
            `  (BuildTarget, HashCode)` pairs for all root build targets
            and their dependencies.
            :::

            [Throws:]{.throwsLabel}
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
