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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.graph](package-summary.html)
:::

## Class ActionAndTargetGraphs {#class-actionandtargetgraphs .title title="Class ActionAndTargetGraphs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.graph.ActionAndTargetGraphs

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ActionAndTargetGraphs
        extends Object

    ::: block
    Container class for
    [`ActionGraphAndBuilder`](../actiongraph/ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph")
    and
    [`TargetGraphCreationResult`](../targetgraph/TargetGraphCreationResult.html "class in com.facebook.buck.core.model.targetgraph").
    Also contains helper methods to choose which
    [`TargetGraph`](../targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    to use
    ([`VersionedTargetGraph`](../../../versions/VersionedTargetGraph.html "class in com.facebook.buck.versions")
    vs un-versioned).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `ActionAndTargetGraphs()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract A           | `getAct               |                       |
        | ctionGraphAndBuilder` | ionGraphAndBuilder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Targe                | `getTargetGraph()`    | ::: block             |
        | tGraphCreationResult` |                       | Helper method to get  |
        |                       |                       | the appropriate       |
        |                       |                       | [`TargetGraph`](.     |
        |                       |                       | ./targetgraph/TargetG |
        |                       |                       | raph.html "class in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Targe         | `getTargetGr          | ::: block             |
        | tGraphCreationResult` | aph​(TargetGraphCreati | Helper method to      |
        |                       | onResult unversionedT | choose versioned vs   |
        |                       | argetGraph,           | un-versioned          |
        |                       |      Optional<TargetG | [`TargetGraph`](.     |
        |                       | raphCreationResult> v | ./targetgraph/TargetG |
        |                       | ersionedTargetGraph)` | raph.html "class in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Targe       | `getUnve              |                       |
        | tGraphCreationResult` | rsionedTargetGraph()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getVe                |                       |
        | tract Optional<Target | rsionedTargetGraph()` |                       |
        | GraphCreationResult>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `of                   |                       |
        | .facebook.buck.core.m | ​(TargetGraphCreationR |                       |
        | odel.graph.ImmutableA | esult unversionedTarg |                       |
        | ctionAndTargetGraphs` | etGraph,   Optional<? |                       |
        |                       |  extends TargetGraphC |                       |
        |                       | reationResult> versio |                       |
        |                       | nedTargetGraph,   Act |                       |
        |                       | ionGraphAndBuilder ac |                       |
        |                       | tionGraphAndBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### ActionAndTargetGraphs

                public ActionAndTargetGraphs()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnversionedTargetGraph()}

        -   #### getUnversionedTargetGraph

            ``` methodSignature
            public abstract TargetGraphCreationResult getUnversionedTargetGraph()
            ```

        []{#getVersionedTargetGraph()}

        -   #### getVersionedTargetGraph

            ``` methodSignature
            public abstract Optional<TargetGraphCreationResult> getVersionedTargetGraph()
            ```

        []{#getActionGraphAndBuilder()}

        -   #### getActionGraphAndBuilder

            ``` methodSignature
            public abstract ActionGraphAndBuilder getActionGraphAndBuilder()
            ```

        []{#getTargetGraph(com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,java.util.Optional)}

        -   #### getTargetGraph

            ``` methodSignature
            public static TargetGraphCreationResult getTargetGraph​(TargetGraphCreationResult unversionedTargetGraph,
                                                                   Optional<TargetGraphCreationResult> versionedTargetGraph)
            ```

            ::: block
            Helper method to choose versioned vs un-versioned
            [`TargetGraph`](../targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph").
            :::

        []{#getTargetGraph()}

        -   #### getTargetGraph

            ``` methodSignature
            public TargetGraphCreationResult getTargetGraph()
            ```

            ::: block
            Helper method to get the appropriate
            [`TargetGraph`](../targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph").
            :::

        []{#of(com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,java.util.Optional,com.facebook.buck.core.model.actiongraph.ActionGraphAndBuilder)}

        -   #### of

            ``` methodSignature
            public static com.facebook.buck.core.model.graph.ImmutableActionAndTargetGraphs of​(TargetGraphCreationResult unversionedTargetGraph,
                                                                                               Optional<? extends TargetGraphCreationResult> versionedTargetGraph,
                                                                                               ActionGraphAndBuilder actionGraphAndBuilder)
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
